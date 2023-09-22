# Lecture Note

***Note*** : this Document is note about git shell command

## Shell command List
- ### pwd : shows the current path in a hierarchical directory
- ### cd : change directory
  - #### argument
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
    - -l : show detailed information(long format)
    - -lh : same as above, but size in units
    - /bin : list the files in the /bin directory
    - -la : list all files(even ones with names beginning with a period character, which are normally hidden)
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
  - Autocompletion : press "tab" key
  - Past commands : press "up arrow" key

## Manipulation
- cp
- mv
- rm
- mkdir
