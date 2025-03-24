#  Basics of Terminal

## 1. Introduction to Terminal and Shell
- The Terminal (or command-line interface) allows users to interact with their system using commands instead of a graphical interface.
- A Shell (e.g., Bash, Zsh, PowerShell) is the command interpreter that processes these commands.

## Check your shell type using:
```sh
echo $SHELL
```


## 2. Basic Shell Commands
- **echo** – Prints text to the terminal:


  ```sh
  echo "Hello, World!"
```
- **pwd** – Displays the current directory:

```sh
pwd
```

whoami – Shows the logged-in user
```sh
whoami
```

## 3. Navigating the File System (cd)
cd (Change Directory) is used to move between folders.
```sh
cd /home/user/Documents
cd ..
cd ~  # Go to home directory
```

## 4. Listing Directory Contents (ls)
```sh
ls
ls -l  # Detailed list
ls -a  # Show hidden files
```

## 5. Creating, Copying, Moving, and Deleting Files and Directories
```sh
touch file.txt  # Create a file
mkdir my_folder  # Create a directory
```

Copying and Moving
```sh
cp file.txt backup.txt  # Copy file
mv file.txt new_location/  # Move file
```

Deleting files and directories
```sh
rm file.txt  # Delete file
rmdir my_folder  # Remove empty folder
rm -r my_folder  # Remove folder with contents
```

## 6. Viewing and Editing Files
```sh
cat file.txt //view file content
nano file.txt // simple text editor
vim file.txt //advance text editor
```
Writing a File Using nano
```sh
nano filename.txt
// Press CTRL + X (Exit)
//Press Y (Yes) to confirm saving the file.
//Press Enter to confirm the filename.
```
Writing and Saving a File in vim
```sh
vim filename.txt
// :w - Save (write) the file without exiting
:q	Quit (if no changes were made)
:q!	Quit without saving (force exit)
:wq!	Save and exit (force save if needed)
```

## 7. What Is Prompt in Terminal?
The prompt is the line where you enter commands.
Default format:
```sh
user@hostname:~$
```

you can customize it using:
  ```sh
PS1="CustomPrompt> "
```


## 8. Configuring Our Terminal Using .bashrc File
.bashrc is a configuration file for Bash shell that runs every time a terminal session starts.
You can edit it to set aliases, modify the prompt, and customize the shell.

```sh
nano ~/.bashrc
```
Example customization:
```sh
export PATH=$PATH:/new/path
```

Modify .bashrc, save changes, and reload using:
```sh
source ~/.bashrc
```

## 9. Using Aliases for Command Shortcuts (alias)
Aliases let you create shortcuts for commands.
```sh
alias ll="ls -lah"
alias gs="git status"
```
To make them permanent, add them to ~/.bashrc.


