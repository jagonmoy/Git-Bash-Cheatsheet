
- ### For making a Directory : 
      mkdir directory_name 
- ### For Changing the Directory : 
      cd directory_name 
- ### Going back to previous directory
      cd ..
- ### Going back to root directory
      cd ../
- ### For showing all the directories/files in current path
      ls
- ### For Creating a file in a directory/folder : 
      touch filename.fileExtension
- ### For Getting Path of Current directory
      pwd
- ### For clearing all the command history
      clear
- ### For initializing a git repository : 
      git init
- ### For Cloning A repository : 
      git clone HTTPS_link_of_GITHUB_repository
- ### For showing all the changes made in a repository : 
      git status
- ### For staging a particular file which is not staged :
      git add filename.fileExtension
- ### For staging all the files 
      git add -A
  ### or
      git add --all
- ### For staging all the files which are descendant of current directory
      git add .
- ### For staging all the files except the deleted files
      git add *.fileExtension
- ### For staging all the files of a similar type
      git add 

  ### One may think that "git add ." and "git add --all" are same . But They are not same If current directory is a root directory then "git add ." and "git add --all" will be same otherwise they are not same . "git add ." only stage the files which are descendant of current directory <br><br>
- ### For unstaging all the staged files 
      git reset
- ### For commiting Locally : 
      git commit     
  ### or 
      git commit -m "Reason for Commit" 
  ### or 
      git commit -m "Reason for Commit" -m "description of commit"
- ### For Unstaging all the committed files 
      git reset HEAD~
- ###  For getting the deleted files back
      git reset --hard
- ### For deleting a file which is staged after updating / not totally updated 
      git rm fileName.fileExtension
- ### For deleting a file forcefully ( That means the file is not staged after updating)
      git rm fileName.fileExtension -f
- ### file will not be deleted in actual working directory but it will be showed in the commit that it is deleted
      git rm --cached fileName.fileExtension
- ### for deleting all the files in the folder
      git rm folderName
- ### for deleting all the files/directories that are descendant to the folder
      git rm -r folderName


   
   
   
       
        
