# VITMAS_Task0_21MID0229

# Git Commands

### Configuring Git

- Configures the **global username**  
  
        git config --global user.name "Aravind S"

- Configures the **global email address** of the user  

        git config --global user.email "ara7ind@gmail.com"

- To set ***VS code*** as the **default editor**  
( --wait : terminal waits untilvs code is closed)  

        git config --global core.editor "code --wait"

- To **edit the global settings** in a text editor
  
        git config --global -e

- To handle **end of lines** in each OS
    - Linux and macOS  

            git config --global core.autocrlf input
    - WINDOWS  

            git config --global core.autocrlf true

- To get **help**  

        git config --help
        git config -h


### Initalizing a Repository

- Creating a **new directory**

        mkdir "folder_name"
        cd "folder_name"

- Initialize a **empty repository**

        git init

- To **view** the contents of that folder

        ls
        ls -a

- To **open** the .git file  

        open .git

- To **delete** the .git file  

        rm -rf .git

## Git Workflow  

### Staging Files 

- To see the **status** of the working directory

        git status

- To add the files in the directory to the staging area

    - To add files by their name  

            git add "file1_name" "file2_name"  
    - To add same type of files  

            git add "*.extension_name"  
    - To add all the files in that diretory  

            git add . 

- To see files in the staging area  
  
        git ls-files  

### Commiting Changes  

- To commit the files in the staging area to github repository

        git commit -m "commit_message"

- To give a long commit message.(This will open the default text editor where we can type our message)

        git commit

- Commit the files without staging them

        git commit -a -m "Commit without staging"

### Removing the files

- To remove a file in the directory

        rm "file1_name"

- To reflect that in the staging area and commit the changes

        git add "file1_name"  
        git commit -m "removed file1_name"

- To delete a file both in directory and staging area

        git rm "file1_name"  

### Renaming or Moving the files

- To rename / move file in a directory

        mv "old_file_name" "new_file_name"
        git add "old_file_name"
        git add "new_file_name"

- Alternative Command

        git mv "old_file_name" "new_file_name"
        git commit -m "file renamed/moved "
