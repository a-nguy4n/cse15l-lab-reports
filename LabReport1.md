# Lab Report #1: Remote Access and FileSystem 

Beginning to remote access and figuring out how to login into a course-specific 
account can seem quite troublesome. However, that can now easily be resolved through 
these simple steps!


## VScode Installation 

**First, VScode must be installed onto the computer.** 
* I did not complete this specific step exactly, as prior to the lab, VScode had
already been installed in my Mac.

**Once VScode is installed, when the application is open, it should open to this:**

![Image](VSCode.png)

<br/>


**However for those on a different Operating System (OS), the setup will differ:** 

![Image](VSCodeOS.png)

+ __For MacOS:__
  After downloading VScode for MacOS specifically, next is to launch it. 
  1. Open Command Palette by pressing the keys: Command + Shift + P
  2. Next, type in : shell command 
  3. Then, install 'code' command in PATH command <br/>


  More specific instructions can be found here: [link](https://code.visualstudio.com/docs/setup/mac)

+ __For Windows x64:__
 After downloading VScode for Windows specifically, next is to launch it. 
 The launch for Windows will differ to that of Mac as to set up and launch, 
 it is important to run the installer: VSCodeUserSetup-{version}.exe More specific instructions can be found here: [link](https://code.visualstudio.com/docs/setup/windows)

+ __For Linux x64:__ 
After downloading VScode for Linux specifically, next is to launch it. 
Launching VScode for Linux will be different to Windows and MacOS due to 
installation for Debian/Ubuntu based distributions or running different commands.More specific instructions can be found here: [link](https://code.visualstudio.com/docs/setup/linux) 



## Remote Connection 

**Before remote connection:**

1) Look up specific-course account for CSE15L here: [link](https://sdacs.ucsd.edu/~icc/index.php)

2) Login. Then, click on the course for CSE15L. It typically starts with: cs15l.

3) Next, use the Global Password Change Tool to reset your password. This will be important
   for the remote connection as well as the shown username.
   
4) Remember your password and username for remote connection.

   
   
   
**To Remote Connect:**
   
1) Open VScode. Then open the terminal using the command: ctrl + ` 

2) Now that the terminal is open, type in ssh **username**@ieng6.ucsd.edu

3) If entered correctly, the next line would ask a question whether
   to continue connecting. Type in: yes
   
4) Then, enter your password that you've reset your account to.
   * Note: When typed in the terminal it won't show up because it is invisible.
   
5) When the password has been inputted correctly, the terminal should show:
 
   ![Image](RemoteLogin.png)
    

   
   
## Running Some Commands 
**Now that you've successfully remotely connected, run some commands.**


**cd Command:**

>![Image](cdCommand.png)

The cd command is meant to switch what is the current directory to a specified path. This means 
you can navigate to another folder on your computer. 


**pwd Command:**
 
 >![Image](PWDcommand.png)
 
 Here the pwd command prints out what is the current working directory, the folder you are working
 in at the moment. 
 
 
**ls -lat Command:**
  
  >![Image](lsLATcommand.png)
  
  This command results in a list of the files in the current working directory as shown above.<br/>
  
  
  Here is a breakdown of the command components: 
  * __ls__ simply lists the directory contents 
  * __l__ refers to setting the output in a list format 
  * __a__ specifies the command to not ignore any files that begin with: .  and  .. 
  * __t__ sorts the files by time, where the newest files are listed in the beginning 
 
