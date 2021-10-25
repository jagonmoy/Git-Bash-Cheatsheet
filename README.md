
[Excellent Bengali Crash Course for Learning Git and GitHub](https://www.youtube.com/watch?v=oe21Nlq8GS4)


- ### opening visual studio Code
      code
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
      git add *
- ### For staging all the files of a similar type
      git add *.fileExtension

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
- ### For getting the deleted files back
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
- ### For showing all the branches 
      git branch
- ### For creating a branch 
      git branch branch_name
  ### When we create a new branch it contains all the directories/files from it's current branch <br><br>
- ### For Switching a Branch 
      git checkout branch_name
- ### For renaming a Branch both locally and remotely
    ### Step 01: <br><br>
    ### Start by switching to the local branch which you want to rename:
      git checkout "old_name"
    ### Step 02: <br><br>
    ### Rename the local branch by typing:
      git branch -m "new_name"
    ### Step 03 : <br><br>
    ### At this point, you have renamed the local branch.

    ### If you’ve already pushed the "old_name" branch to the remote repository , perform the next steps to rename the remote branch.

    ### Push the <new_name> local branch and reset the upstream branch:
      git push origin -u "new_name"
    ### Step 04: <br><br>
    ### Delete the "old_name" remote branch:
      git push origin --delete <old_name>


- ### If we make any changes that can be updating,inserting or deleting a file in a branch and commit it , then it doesn't affect the other branches. If we visit other branches we will not see any changes there though we made some changes in our previous branch.

- ### Suppose In our System There is two branches , One is Branch_1 and other one is Branch_2  . In Branch_1 we made a change in file1.txt and in Branch_2 we made a change in file2.txt . Now I am in Branch_1 and I also like to include the changes in file2.txt which was made in Branch _2 . How to do it ??? We can use git merge to do it .
      git merge branch_2 -m "Some message"
  ### or
      git merge branch_2
  ### Now Branch_1 will also include the changes made in Branch_2 . Same process applies for Branch_2 also if we want to include the changes made in Branch_1.
      git merge branch_1 -m "Some message"
  ### or
      git merge branch_1

- ### Now Suppose In our system from both of our branches Branch_1 and Branch_2 we made a change in a single file file1.txt . Now is it possible to merge ??? 
  ### No , If we try to merge then It will show us a error message and will suggest us to resolve the merge conflict . After resolving the Conflict it will be possible to merge . <br> <br>

- ### After doing Commit How to Push all the changes we made in local repository to remote reopository .
      git push origin branch_name
- ### Now Suppose We made some changes in our remote repository and we would like to get this changes in our working directory . How to do it ? We can do it in two way one is by 'fetch' and other way is by 'pull'
     - ### fetch : 'fetch' can get all the changes made in remote repository to our local repository but not in our working directory . So just doing the fetch command we will not be able to see the changes in our working directory . For this we will also have to another merge command. So the command will be 
       ### Step 1 : 
             git fetch origin branch_name
       ### or 
             git fetch
       ### Step 2 :
             git merge origin branch_name
       ### or 
             git merge
   - ### pull : 'pull' can get all the changes direct to our working directory unlike remote repository . We don't have to merge .
         git pull origin branch_name
     ### or 
         git pull
     
     

      




   
   
   
       
        
