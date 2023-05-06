# Lab Report #3: Researching the Command - *find*
This report will look into the command *find* and address alternate ways to use this command. 

## What is the command *find* ? 
The command *find* is used to search for files and directories based on distinct characteristics
like size, type, date, etc. 

**Syntax:**  find [path] [expression]
  - path narrows the scope and defines where find will search
  - expression consists of patterns, options to search specifically for what file or directory

## Ways to Use *find* 
Here, there will be some command-line options exploring the use of *find* in the terminal. 
 - find -type
 - find -regex 
 - find [directory name] -type f -mtime [some time #] 
 - Alternate to find: locate [some pattern] 

## find -type
- Using find -type allows the user to search for specific filetypes. 

**Example 1:** find -type d
- This command allows the user to lookup all the directories in their current working directory. It is useful as it
  allows the user to look into the directory hierarchy and manipulate it, such as changing the directories permissions. 
- [Source](https://linuxize.com/post/how-to-find-files-in-linux-using-the-command-line/)

- Input 
  ```
  find -type d
  ```
- Output 
  ```
  .
  ./911report
  ./biomed
  ./government
  ./government/About_LSC
  ./government/Alcohol_Problems
  ./government/Env_Prot_Agen
  ./government/Gen_Account_Office
  ./government/Media
  ./government/Post_Rate_Comm
  ./plos
  ``` 
**Example 2:** find -type f -size -[some size]
- This command allows the user to lookup files in their current working directory with this specific size range. It is particularly useful in 
  finding a range of small or large files and finding files that are taking too much space (for deletion). 
- [Source](https://linuxize.com/post/how-to-find-files-in-linux-using-the-command-line/)

- Input 
  ```
  find -type f -size -1024c
  ```
  
- Output
  ```
  ./plos/pmed.0020191.txt
  ./plos/pmed.0020226.txt
  ```
  
 ## find -regex 
 
 - Using find -type allows the user to search for specific filetypes with the given pattern. This is useful because users can now easily
 lookup certain specific group of files that contain that given pattern. 

**Example 1:**  find -regex .* bcr.*
- This command results in finding all specific files that contain the pattern: bcr. It is useful as the user can now focus and find the specific
 file that contains the bcr pattern instead of looking through an entire list of files. 
- [Source](https://www.baeldung.com/linux/find-command-regex)

- Input 
  ```
  find -regex .*bcr.*
  ```
- Output (shortened) 
  ```
  ./biomed/bcr273.txt
  ./biomed/bcr284.txt
  ./biomed/bcr285.txt
  ./biomed/bcr294.txt
  ./biomed/bcr303.txt
  . . . (more files)
  ``` 
  
**Example 2:** find [directory name] -regex .* txt.* 
- The user can also narrow down which directory to find files from and search for files that end with '.txt'. This is useful
  in determining how many of that file type is there or what file type the user wants to access. 
- [Source](https://www.baeldung.com/linux/find-command-regex)

- Input 
  ```
  find 911report/ -regex .*txt.*
  ```
  
- Output (shortened)
  ```
  911report/chapter-1.txt
  911report/chapter-10.txt
  911report/chapter-11.txt
  911report/chapter-12.txt
  911report/chapter-13.1.txt
  . . . (more files) 
  ```


## find [directory name] -type f -mtime [some time #] 
 - Users can find files within the given range of modification time. This is useful in accessing and finding files recently modified or modified since
 the last given time.  

**Example 1:**  find government/ -type f -mtime -3
- This command results in finding all specific files have been modified in less than three days within the government directory.This is useful in finding   files that have been modified or accessed recently.
- [Source](https://www.makeuseof.com/find-command-linux/)

- Input 
  ```
  find government/ -type f -mtime -3
  ```
- Output (shortened) 
  ```
  government/Media/Oregon_Poor.txt
  government/Media/Owning_a_Piece.txt
  government/Media/Paralegal_Honored.txt
  government/Media/Philly_Lawyers.txt
  . . . (more files)
  ``` 
  
**Example 2:** find biomed/ -type f -mtime +1
- This command results in finding all specific file having been modified more than 1 day in the biomed directory. This is useful in finding files
  that haven't been modified or accessed in a longer time.
- [Source](https://www.makeuseof.com/find-command-linux/)

- Input 
  ```
  find biomed/ -mtime +1
  ```
  
- Output (shortened)
  ```
  biomed/1471-2091-2-5.txt
  biomed/1471-2091-2-7.txt
  biomed/1471-2091-2-9.txt
  biomed/1471-2091-3-13.txt
  . . . (more files) 
  ```
  
## locate [pattern/option]
 - The command locate is an alternative to find and it will search the locate database. Then it will return a list of all files and 
  directories that match the search term or given pattern.

**Example 1:** locate 11.txt
- This command results in finding all specific files that contains the pattern "11.txt" and the root path. Like the command find, it is useful in searching for files with
  only a specifc term that narrows down the search for users. 
- [Source](https://linuxize.com/post/locate-command-in-linux/#:~:text=The%20syntax%20for%20the%20locate,%5BOPTION%5D%20PATTERN...&text=In%20its%20most%20basic%20form,the%20user%20has%20read%20permission.)

- Input 
  ```
  locate 11.txt
  ```
- Output (shortened) 
  ```
  /etc/pki/nssdb/pkcs11.txt
  /usr/share/doc/git-2.39.2/RelNotes/1.7.11.txt
  /usr/share/doc/git-2.39.2/RelNotes/2.4.11.txt
  /usr/share/doc/libsrtp-1.4.4/rfc3711.txt
  /usr/share/doc/openldap-devel-2.4.44/rfc/rfc4511.txt
  . . . (more files)
  ``` 
  
**Example 2:** locate -S
- This command shows the locate database stats. It is useful when the user is unsure of their current status of their mlocate.db
- [Source](https://www.tecmint.com/linux-locate-command-practical-examples/)

- Input 
  ```
  locate -S
  ```
  
- Output 
  ```
  Database /var/lib/mlocate/mlocate.db:
        38736 directories
        367939 files
        20320690 bytes in file names
        8947450 bytes used to store database
  ```
  
  
  
  
 

 
 
