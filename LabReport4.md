# Lab Report #4: Vim Command Line Task 
This lab report will be a step-by-step process of forking a repository, cloning the repository, 
and using VIM to edit and save the file. 

## Step 1: Setup - Delete any existing forks of the repository you have on your account
  
  1) Go into your GitHub account and into the repository.
  <br>
   
   
  2) Go to the repository's settings 
     > ![Image](GitSettings.png)
  <br>
  
  
  3) Scroll all the way down and click on the button 'Delete this repository'. 
     This will delete any exiting forks of the repository. 
     > ![Image](DeleteRepos..png)
  <br>
  
  
  4) Additionally, log into the @ieng6 account. Then use the command **rm -r lab7/** to remove the directory
     from the account in order to follow the next steps. When completed logout of the account.  
     > ![Image](RemoveLab7.png)
<br>


## Step 2: Setup - Fork the repository

  1) Follow this [link](https://github.com/ucsd-cse15l-s23/lab7) to fork Lab 7's repository. 
    >![Image](Forking7.png)
<br>


## Step 3: Start the timer!

  1) Begin a timer to determine your baseline in logging in, cloning, and editing the code. 
<br>


## Step 4: Log into ieng6

  1) Use the command: **ssh cs15lsp23__@ieng6.ucsd.edu** to remote login. 
  ```
  ssh cs15lsp23il@ieng6.ucsd.edu
  ```
  
  - With ssh you can remote login to your account in order to begin the cloning process of the repository.
    

<br>


## Step 5: Clone your fork of the repository from your Github account
1) Use the command: **git clone < ssh link >** to clone the repository from your GitHub account into your ieng6 account
  ```
  git clone git@github.com:a-nguy4n/lab7.git
  ```
2) Use the command **ls** to check if the repository has been cloned into the account. The directory name **lab7** should be listed. 
   > ![Image](Lab7Check.png)



3) Then, use the command **cd** to get into the repository and access its files. 
  ```
  cd lab7/
  ```

4) Once the directory has changed into that repository, use command **ls** to see the files inside. 
   > ![Image](Lab7LS.png)


<br>


## Step 6: Run the tests, demonstrating that they fail

<br>


## Step 7: Edit the code file to fix the failing test

<br>


## Step 8: Run the tests, demonstrating that they now succeed


## Step 9: Commit and push the resulting change to your Github account (you can pick any commit message!)
