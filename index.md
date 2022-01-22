# Lab 1 Instructions

## by Pranav Mekkoth

![Image](https://user-images.githubusercontent.com/97641097/149264783-048d359e-8193-4f02-bda2-4418517178af.png)

**For this Lab, you will need to follow each of the links below. Each link corresponds to 1 step you will need to complete in order to finish this lab. Each step will include instructions for what you should do.**

If you have any questions regarding the instructions to the lab, contact the instructor or a TA.

**Steps:**
* **Step 1: Installing VScode**

    **Instructions:**
    1. Go to the Visual Studio Code Website ([VScode](https://code.visualstudio.com/download)) and follow the instructions to download the appropriate version for your computer.
    2. Open Visual Studio Code on your computer

    This is what it should look like afterwards:
    ![Image](https://user-images.githubusercontent.com/97641097/149268597-3ee23a7e-7b68-44ad-9ce0-a864fe694677.png)

* **Step 2: Remotley Connecting**

    **Instructions:**
    1. If you have a Windows computer install Open SSh ([link](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)). Then, look up your course specific accound: [ucsd accounts website](https://sdacs.ucsd.edu/~icc/index.php).
    2. Open a new Terminal in VScode. 
    3. Type: `ssh [your course specific account]` in the terminal window. When a message asks "Are you sure you want to continue connecting?" enter `yes`. You will then be prompted to enter your password (no text will show up while typing password). 

    At this point, you are connected to the CSE 15L server.

    ![Image](https://user-images.githubusercontent.com/97641097/149273040-1c1fdc38-20f6-4ea2-9e93-b339f682770b.JPG)


* **Step 3: Try some commands**

    **Instructions:**
    1. Try running commands like `cd`, `ls`, `pwd`, `mkdir`, `cp`, and any other useful commands in the terminal of your computer and the server.
    2. Experiment with a couple of these useful commands for yourself: `cd~`, `ls-lat`, `ls-a`, `ls-directory` .

    Example result:

    ![Image](https://user-images.githubusercontent.com/97641097/149273846-90ee8747-65a4-4733-9457-e4c00678d0fd.JPG)

* **Step 4: Moveing files with scp**
   
   **Instructions:**
   
   1. Create a file called WhereAmI.java with the following code. (first image under the instructions)
   2. In the terminal directory where you made the file, run the following command: `scp WhereAmI.java [your ucsd course account] :~/`. You will be prompted to enter your password to log into the server.
   3. When you are in the server, enter `ls` in the terminal to confirm the files has been copied over. Then, use appropriate commands to run the code (javac then java).
  
  ![Image](https://user-images.githubusercontent.com/97641097/149275523-f3e05dc5-8c07-4cba-aac2-cb8253abf232.png)

    The end result should look similar to this:

    ![Image](https://user-images.githubusercontent.com/97641097/149274979-9f3c96e6-f965-4ce1-9c8b-c72a14e64966.JPG)

* **Step 5: Setting a SSH key**

    **Instructions:**
    
    1. (in the VScode terminal for your computer) enter `ssh-keygen` command. Follow to the prompts and answer the necessary questions. This should result in creating a pair of public and private keys tha will allow you to log into the server for the class without entering your password every time. 
    2. If you are on windows, go to this [link](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation) to do the additional `ssh-add` commands.
    3. Log into the class server (with your account). Run the command `mkdir .ssh` in the server terminal than logout of the server. Now you should be able to enter the server without haveing to enter a password.

    Logging in should look similar to this:

    ![Image](https://user-images.githubusercontent.com/97641097/149276921-d3f25558-7ea9-4dc5-a33e-5d8ccfd2cf2b.png)

* **Step 6: Optimizing remote running**

    **Instructions:**
    1. Experiment with running commands in the terminals of your compter(on VScode) and on the server to find shortcuts and quicker ways to do things. 
    2. Hints: You can run a ssh command with quotes at the end to run it directly on your server. You can also use semicolons to run multiple commmands on the same line. You can also use the up arrow key to find/run previously used commands.

     What we tried as a group:
     1. Edit the file:
        
        ![Image](https://user-images.githubusercontent.com/97641097/150620497-694bacc2-9f66-4ca1-ac6a-0181b070d464.JPG)
      
     2. Use the up arrow keys to compile and run the program:
        
        ![Image](https://user-images.githubusercontent.com/97641097/150620766-eb0548b0-a852-450d-9998-043d38c02ff6.png)
        
     3. Use the up arrow keys agian to run it in the server without log into the server:
      ![Image](https://user-images.githubusercontent.com/97641097/150620872-4df35182-9a89-4f58-a81b-5b8a76fa884f.png)
      


**Now that you have completed all 6 steps, you are now finished with CSE 15L lab 1!**
