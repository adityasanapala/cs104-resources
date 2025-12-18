
## **Unix CLI Basics**

### **1. Understanding the File System Hierarchy**

Unix organizes files in a hierarchical structure starting from the **root directory** `/`. Common directories include:

* `/bin` – essential system binaries (e.g., `ls`, `cp`)
* `/home` – user home directories
* `/etc` – configuration files
* `/var` – variable data (logs, databases)
* `/tmp` – temporary files
* `/usr` – user binaries, libraries, and documentation

### **2. Navigating the File System**

* `pwd`
  **Print Working Directory**: Displays the current directory.

* `cd <dir>`
  **Change Directory**: Navigates to a directory.
  Examples:

  * `cd /home/user`
  * `cd ..` (go up one directory)
  * `cd ~` (go to home directory)

* `ls`
  **List Files**: Displays files in the current directory.
  Useful options:

  * `ls -l` (detailed list)
  * `ls -a` (includes hidden files)
  * `ls -lh` (human-readable file sizes)

### **3. Managing Files and Directories**

* `touch <filename>`
  Creates an empty file.

* `mkdir <dir_name>`
  Creates a new directory.

* `cp <source> <destination>`
  **Copy** files or directories.
  Example: `cp file1.txt file2.txt`

* `mv <source> <destination>`
  **Move** or **Rename** files or directories.
  Example: `mv oldname.txt newname.txt`

* `rm <file>`
  **Remove** a file.
  For directories:

  * `rm -r <dir>` (recursively remove a directory)

* `rmdir <dir>`
  Remove an empty directory.

### **4. Viewing and Editing Files**

* `cat <file>`
  **Concatenate and display** the content of a file.

* `more <file>`
  View the content of a file, page by page.

* `less <file>`
  Similar to `more`, but allows backward navigation.

* `head <file>`
  Display the first 10 lines of a file.

* `tail <file>`
  Display the last 10 lines of a file.

* `nano <file>`
  Open a file in the **nano** text editor (a simple terminal editor).

* `vi <file>`
  Open a file in the **Vi** editor (more complex).

### **5. Searching and Finding Files**

* `find <dir> -name <filename>`
  Find files by name.
  Example: `find /home -name "*.txt"`

* `grep <pattern> <file>`
  Search for a **pattern** within a file.
  Example: `grep "error" logfile.txt`

* `locate <filename>`
  Find files using a pre-built index (faster than `find` but requires an updated database).

### **6. File Permissions**

Unix is a multi-user system with file permissions that define who can read, write, or execute files:

* `ls -l`
  View file permissions (e.g., `-rwxr-xr-x`):

  * `r` (read)
  * `w` (write)
  * `x` (execute)

* `chmod <permissions> <file>`
  Change file permissions.
  Example: `chmod 755 file.txt` (rwxr-xr-x)

* `chown <owner>:<group> <file>`
  Change file ownership.
  Example: `chown user:admin file.txt`

* `chgrp <group> <file>`
  Change file group.

### **7. Process Management**

* `ps`
  Display currently running processes.

* `top`
  Interactive process viewer.

* `kill <pid>`
  Kill a process by its **Process ID** (PID).
  Example: `kill 1234`

* `killall <process_name>`
  Kill all processes with a given name.

* `bg`
  Send a job to the background.

* `fg`
  Bring a job to the foreground.

### **8. Redirection and Pipes**

* `>`
  Redirect output to a file, overwriting it.
  Example: `echo "Hello, World" > file.txt`

* `>>`
  Append output to a file.
  Example: `echo "New line" >> file.txt`

* `<`
  Redirect input from a file.
  Example: `sort < file.txt`

* `|`
  Pipe output of one command as input to another.
  Example: `ls -l | grep ".txt"`

### **9. Environment Variables**

* `echo $<variable>`
  Display the value of an environment variable.
  Example: `echo $HOME`

* `export <variable>=<value>`
  Set an environment variable.
  Example: `export PATH=$PATH:/new/directory`

### **10. Working with Archives and Compression**

* `tar -czvf archive.tar.gz <dir>`
  Create a compressed archive using `tar`.
  Example: `tar -czvf backup.tar.gz /home/user/`

* `tar -xzvf archive.tar.gz`
  Extract a compressed archive.

* `gzip <file>`
  Compress a file.

* `gunzip <file.gz>`
  Decompress a file.

### **11. Networking Commands**

* `ping <host>`
  Check connectivity to a host.

* `ifconfig`
  Display network configuration (older systems).

* `ip addr`
  View network interfaces and their IP addresses.

* `netstat`
  Display network connections, routing tables, etc.

* `scp <source> <user>@<host>:<destination>`
  Secure copy a file over SSH.

### **12. Useful Shortcuts**

* `Ctrl + C`
  Terminate a running command.

* `Ctrl + Z`
  Suspend a process (can be resumed with `fg`).

* `Tab`
  Auto-completion of commands and filenames.

* `Ctrl + R`
  Reverse search through command history.

* `!!`
  Re-run the last command.

