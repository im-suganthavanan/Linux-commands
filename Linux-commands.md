# Linux-Commands-Cheatsheet

Creating this repo with an intent to make Linux commands easy for beginners. This is a work-in-progress repo.

## Navigation & Directory Basics

Commands to move around and check where you are in the filesystem.

1. `pwd` - Print the current working directory
2. `ls` - List files and folders in the current directory
3. `ls -la` - List all files, including hidden ones, with details
4. `cd <dir_name>` - Change directory
5. `cd ..` - Move one directory up
6. `cd ~` - Go to the home directory
7. `cd -` - Go back to the previous directory

## File & Directory Management

Commands to create, copy, move, and delete files or folders.

1. `mkdir <dir_name>` - Create a new directory
2. `mkdir -p <dir_name>/<nested_dir_name>` - Create nested directories in one go
3. `touch <filename>` - Create a new empty file
4. `cp <source> <destination>` - Copy a file or directory
5. `cp -r <source_dir> <dest_dir>` - Copy a directory recursively
6. `mv <source> <destination>` - Move or rename a file/directory
7. `rm <filename>` - Delete a file
8. `rm -r <dir_name>` - Delete a directory and its contents
9. `rm -rf <dir_name>` - Force delete without confirmation (use with caution)

## Viewing & Editing Files

Commands to read, write, and edit file contents.

1. `cat <filename>` - Display the contents of a file
2. `cat > <new_file>` - Create a new file and write content (Ctrl+D to save)
3. `cat >> <file>` - Append content to an existing file
4. `echo "text"` - Print text to the terminal
5. `echo "text" > <file>` - Write text into a file (overwrite)
6. `echo "text" >> <file>` - Append text to a file
7. `nano <filename>` - Open a file in the Nano editor
8. `vi <filename>` - Open a file in the Vi/Vim editor
9. `head <filename>` - View the first 10 lines of a file
10. `tail <filename>` - View the last 10 lines of a file
11. `tail -f <filename>` - Continuously monitor a file for new content

## Searching & Finding

Commands to locate files or text.

1. `find <path> -name "<filename>"` - Search for a file by name
2. `grep "text" <filename>` - Search for a text pattern inside a file
3. `grep -r "text" <dir_name>` - Recursively search for text inside a directory
4. `locate <filename>` - Quickly find files by name
5. `which <command>` - Show the path of an executable command

## Permissions & Ownership

Commands to manage who can access or run a file.

1. `chmod +x <filename>` - Make a file executable
2. `chmod 755 <filename>` - Set specific permissions
3. `chown <user>:<group> <filename>` - Change file owner and group
4. `sudo <command>` - Run a command with admin (root) privileges

## Compression & Archiving

Commands to bundle or unpack files.

1. `tar -cvf <archive.tar> <dir_name>` - Create a tar archive
2. `tar -xvf <archive.tar>` - Extract a tar archive
3. `tar -czvf <archive.tar.gz> <dir_name>` - Create a compressed tar.gz archive
4. `tar -xzvf <archive.tar.gz>` - Extract a tar.gz archive
5. `zip -r <archive.zip> <dir_name>` - Compress a directory into a zip file
6. `unzip <archive.zip>` - Extract a zip file

## Process & System Monitoring

Commands to check what's running and how resources are being used.

1. `ps aux` - Show all running processes with details
2. `top` - Display real-time system resource usage
3. `htop` - Interactive version of top (may need install)
4. `kill <pid>` - Terminate a process by its ID
5. `kill -9 <pid>` - Force kill a process
6. `df -h` - Show disk space usage
7. `du -sh <dir_name>` - Show the size of a directory
8. `free -h` - Show memory (RAM) usage

## Networking

Commands to check connectivity and transfer files over a network.

1. `ping <hostname/IP>` - Check network connectivity to a host
2. `curl <url>` - Fetch data from a URL
3. `wget <url>` - Download a file from the internet
4. `ip a` - Show network interface details and IP address
5. `netstat -tulnp` - Show active connections and listening ports
6. `ssh <user>@<host>` - Connect to a remote machine
7. `scp <file> <user>@<host>:<path>` - Securely copy files to/from a remote machine

## Git & GitHub Basics

Commands used to manage a Git repository.

1. `git init` - Initialize a new Git repository
2. `git clone <url>` - Clone a remote repository locally
3. `git status` - Show the current status of changes
4. `git add <file>` - Stage a file for commit
5. `git add .` - Stage all changed files
6. `git commit -m "message"` - Commit staged changes with a message
7. `git push origin <branch>` - Push commits to a remote branch
8. `git pull origin <branch>` - Pull latest changes from a remote branch
9. `git log` - View commit history

## Miscellaneous

Handy day-to-day utilities.

1. `history` - Show a list of previously used commands
2. `clear` - Clear the terminal screen
3. `alias ll='ls -la'` - Create a custom shortcut for a command
4. `man <command>` - Open the manual page for a command
5. `date` - Display the current date and time
6. `whoami` - Show the current logged-in username
7. `exit` - Close the terminal session

Note: replace anything inside `< >` with your actual value, e.g. `<dir_name>` becomes `my_project`.
