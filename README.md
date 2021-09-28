
### For making a Directory : mkdir folder_name
   ## E.g : mkdir myfolder <br>

### For Cloning A repository : git clone HTTPS_link_of_repository
   ## E.g : git clone https://github.com/jagonmoy/Git-Bash-Cheatsheet.git <br>

### For Changing the Directory : cd directory_name
   ## E.g : Suppose there is a folder "MyFolder"  <br>
        ## cd MyFolder

### For Creating a file in a directory/folder : touch filename.extension
   ## E.g : Suppose I want to create a file name file1.txt in current directory 
      ## touch file1.txt

### For initializing a git repository : git init

### 4. For showing all the files in a repository which were updated,deleted or created : git status
### 5. For Tracking a particular file which is not tracked : git add file_name_with_extension
### 6. For Tracking all the files including Untracked,modified : git add .
   <br> It is recommended to use "git add ." rather than using "git add filename.extension" <br>
### 7. For commiting Locally : git commit -m "Reason for Commit" -m "Description for commit"
### 8. Steps for adding SSH key to Github : 
   Apply these Git commands
   #### Step 1: ssh-keygen -t rsa -b 4096 -C "email_address_added_to_Github" <br>
   #### Step 2: eval $(ssh-agent -s) <br>
   #### Step 3: ssh-add ~/.ssh/id_rsa <br>
   #### Step 4: clip < ~/.ssh/id_rsa.pub <br>
   Now after Copying the Public Key go to Github -> Profile -> Settings -> SSH and GPG Keys and then add <br>
   the ssh key .
 ### 9. For pushing files in Repo : git push origin main/master   
 ### 10. For getting back to Previous Directory : cd ..
 ### 11. What are the steps if we make an repository locally and want it to publish in Github :
   #### Step 1 : git init <br>
   it initialize a git repository in current folder .
   #### Step 2 : git add . <br>
   it trackes all the files .
   #### Step 3 : git commit -m "Reason for Commit" -m "Description for commit" <br>
   for committing locally
   #### Step 4 : Now we will make a repo in GIthub and will copy the SSH link .
   #### Step 5 : git remote add origin SSH_Link <br>
   it will publish the repo live in the github repo
   ####  For checking Step 6 : git remote -v
   #### Step 7 : git push origin main/master <br>
   Finally the repository which we created locally will be published
   
   
   
       
        
