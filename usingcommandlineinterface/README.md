# Command Line Interface (CLI) Guide

## Introduction
The Command Line Interface (CLI) is a powerful tool used to interact with an operating system through text-based commands. It allows users to perform tasks such as file manipulation, process control, system monitoring, and automation efficiently. The CLI is commonly used in Windows (Command Prompt or PowerShell) and Linux (Terminal/Bash).

---

## Using the DOS Command Line (Windows Command Prompt)

### #### Opening Command Prompt
To open the Command Prompt in Windows:
- Press `Win + R`, type `cmd`, and hit `Enter`.
- Search for **Command Prompt** in the Start Menu.
- Open **Run** and type `cmd`.

### #### Basic DOS Commands

- `dir` - Lists files and directories in the current directory.
- `cd [directory]` - Changes the current working directory.
- `mkdir [directory]` - Creates a new directory.
- `rmdir [directory]` - Removes an empty directory.
- `del [filename]` - Deletes a specific file.
- `cls` - Clears the screen.
- `echo [message]` - Prints a message on the screen.
- `exit` - Closes the command prompt.
- `help` - Lists available commands.

### #### File Management in DOS
- `copy [source] [destination]` - Copies a file to a new location.
- `move [source] [destination]` - Moves a file to a new location.
- `ren [oldname] [newname]` - Renames a file.
- `attrib` - Displays or changes file attributes.

### #### System Information and Control
- `ipconfig` - Displays network configuration.
- `tasklist` - Shows running processes.
- `taskkill /IM [processname] /F` - Kills a running process.
- `shutdown /s /t 0` - Shuts down the computer immediately.
- `shutdown /r /t 0` - Restarts the computer immediately.

---

## Using the Linux Terminal

### #### Opening the Linux Terminal
To open a Terminal in Linux:
- Press `Ctrl + Alt + T`.
- Search for **Terminal** in the applications menu.
- Use `tty` to check the terminal session ID.

### #### Basic Linux Commands

- `ls` - Lists files and directories.
- `pwd` - Prints the current working directory.
- `cd [directory]` - Changes the current directory.
- `mkdir [directory]` - Creates a new directory.
- `rm -r [directory]` - Removes a directory and its contents.
- `touch [filename]` - Creates a new empty file.
- `cat [filename]` - Displays the contents of a file.
- `echo "text" > [filename]` - Creates a file with text.
- `clear` - Clears the screen.
- `exit` - Closes the terminal.

### #### File and Directory Management
- `cp [source] [destination]` - Copies a file.
- `mv [source] [destination]` - Moves or renames a file.
- `rm [filename]` - Deletes a file.
- `find /path -name "filename"` - Searches for a file by name.
- `locate [filename]` - Finds the location of a file.

### #### User and System Management
- `whoami` - Displays the current user.
- `id` - Displays user and group ID information.
- `sudo [command]` - Executes a command with root privileges.
- `passwd` - Changes the user password.
- `uptime` - Shows system uptime.
- `top` - Displays real-time system processes.
- `kill [PID]` - Kills a process using its Process ID.
- `shutdown now` - Shuts down the system immediately.

### #### Networking Commands
- `ping [address]` - Tests network connectivity.
- `ifconfig` (or `ip a`) - Displays network interface details.
- `netstat -tulnp` - Shows open ports and active connections.
- `wget [URL]` - Downloads files from a URL.

---

## Command Line Scripting

### #### Writing Batch Scripts (Windows)
A batch script is a sequence of commands stored in a `.bat` file.

Example:
```batch
@echo off
echo Hello, World!
pause
```
Save the file as `hello.bat` and execute it by double-clicking or running `hello.bat` in Command Prompt.

### #### Writing Bash Scripts (Linux)
A Bash script is a set of Linux commands stored in a `.sh` file.

Example:
```bash
#!/bin/bash
echo "Hello, World!"
```
Save the file as `hello.sh`, give it execution permission using `chmod +x hello.sh`, and run it with `./hello.sh`.

---

## Conclusion
The Command Line Interface (CLI) is a powerful tool that allows users to interact with the system efficiently. Whether using Windows Command Prompt or the Linux Terminal, mastering CLI commands can significantly improve productivity and automation capabilities. Learning CLI scripting further enhances the ability to automate tasks and manage systems effectively.

---