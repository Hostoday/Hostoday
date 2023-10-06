## Lecture Note

***Note***: This document is note about Git

## Version and Collaboration
- ### Local
  ![file local](https://velog.velcdn.com/images%2Fjhjeong00%2Fpost%2F488020b6-af3b-4f4c-b048-cc4fff0b4240%2FScreen%20Shot%202021-12-16%20at%203.09.30%20AM.png)
- ### Centralized
  ![file centralized](https://velog.velcdn.com/images%2Fjhjeong00%2Fpost%2F7dbe16d6-3efd-4b27-b1d8-a306e245fab1%2FScreen%20Shot%202021-12-16%20at%203.12.21%20AM.png)
- ### Distributed
  ![file distributed](https://velog.velcdn.com/images%2Fjhjeong00%2Fpost%2Ffc2d62e4-3c53-485b-9951-0dc12a0fdc38%2FScreen%20Shot%202021-12-16%20at%203.15.07%20AM.png)

- ### Three stages in git
  ![file stages](https://codetej.in/wp-content/uploads/2021/05/3-stage-architecture-of-GIt-1024x576.png)

## Git config
- ### Git config level
  - #### system level : --system option. Affects all uses and repositoried on the system(administrative)
  - #### global(user) level : -- global option. Affects all repositories of a current user
  - #### local level : --local option. Specific to the current repository
    **Each level overrides values in the previous level : system -> global -> local**

- ### Command
  - #### git init : Initializing a Repository in an Existing Directory
  - #### git status : Checking Repository Status
  - #### git add[file_name] : Adding a new file to be staged(tracked)
      **if you modify file in stage, you should add that to stage**
  - #### git add . : Adding all files to be staged(tracked)
  - #### git rm -cached[file_name] : Unstaging the file
  - #### nano .gitignore file : ignoring a file
    - *.a : ignore all .a files
    - !lib.a : but do track lib.a, even though you're ignoring .a files above
    - /TODO : only ignore the TODO file in the current directory, not subdir/TODO
    - build/ : ignore all files in any directory named build
  - #### git commit -m "commit massage" : commit
  - #### git branch -m old_name new_name : change branch name
