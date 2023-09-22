# Lecture Note

***Note*** : this Document is note about git shell command

## Shell command List
- ### pwd : shows the current path in a hierarchical directory
- ### cd : change directory
  - #### Argument
    - [directory name]
    - / : root
    - . : current directory
    - .. : upper-level directory
    - ~ : home of current user
    - /[directory name] : absolute path
    - ./[directory name] : relative path
    - ../[directory name] : relative path
- ### ls : list files and directories
  - #### Option
    - -l : Show detailed information(long format)
    - -lh : Same as above, but size in units
    - /bin : List the files in the /bin directory
    - -la : List all files(even ones with names beginning with a period character, which are normally hidden)
      in the parent of the working directory in long format
      ```sh
      -rw-------   1 me       me            576 Apr 17  2019 weather.txt
      drwxr-xr-x   6 me       me           1024 Oct  9  2019 web_page
      -rw-rw-r--   1 me       me         276480 Feb 11 20:41 web_site.tar
      -rw-------   1 me       me           5743 Dec 16  2018 xmas_file.txt

      ----------     -------  -------  -------- ------------ -------------  
      |             |        |         |         |             |
      |             |        |         |         |         File Name
      |             |        |         |         |
      |             |        |         |         +---  Modification Time
      |             |        |         |
      |             |        |         +-------------   Size (in bytes)
      |             |        |
      |             |        +-----------------------        Group
      |             |
      |             +--------------------------------        Owner
      |
      +----------------------------------------------   File Permissions
      Source : https://linuxcommand.org/lc3_lts0030.php
      ```
- ### clear : claer the terminal window
- **Tip**
  - Autocompletion : Press "tab" key
  - Past commands : Press "up arrow" key


## Manipulation
- ### cp : copy files and directories
  - #### Command
    - cp file1 file2 : Copies the contents of file1 into file2. If file2 does not exist, it is created;
      otherwise, file2 is silently overwritten with the contents of file1
    - cp -i file1 file2 : Like above however, since the "-i"(interactive) option is specified, if file2 exists,
      the user is prompted before it is overwritten with the contents of file1
    - cp file1 dir1 : Copy the contents of file1(into a file named file1) inside of directory dir1.
    - cp -R dir1 dir2 : Copy the contents of the directory dir1. If directory dir2 does not exist, it is created. Otherwise, it creates a directory named dir1 within directory dir2.
      
- ### mv : Move files and directories or rename them
  - #### Command
    - mv file1 file2 : If file2 does not exist, then file1 is renamed file2. If file2 exists, its contents are silently replaced with the contents of file1.
    - mv -i file1 file2	: Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1.
    - mv file1 file2 dir1	: The files file1 and file2 are moved to directory dir1. If dir1 does not exist, mv will exit with an error.
    - mv dir1 dir2 : If dir2 does not exist, then dir1 is renamed dir2. If dir2 exists, the directory dir1 is moved within directory dir2.
- ### rm : delete files and directories permantely and irreversevely (Be careful when you are using this command)
  - #### Command
    - rm file1 file2 : Delete file1 and file2.
    - rm -i file1 file2	: Like above however, since the "-i" (interactive) option is specified, the user is prompted before each file is deleted.
    - rm -r dir1 dir2 : Directories dir1 and dir2 are deleted along with all of their contents.
- ### mkdir : Make a new directory


## More Command
- **using help command!**
