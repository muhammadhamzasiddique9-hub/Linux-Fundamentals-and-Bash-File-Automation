# Linux Fundamentals and Bash File Automation

## Overview

This project provides a practical introduction to essential Linux command-line operations and basic Bash scripting. It demonstrates filesystem navigation, file and directory management, command-line operations, executable permissions, and simple task automation.

The project establishes foundational Linux skills that support further learning in system administration, scripting, automation, and cloud computing.

## Objectives

- Understand and execute fundamental Linux commands.
- Navigate the Linux filesystem using the command line.
- Create, copy, move, and remove files and directories.
- Understand basic executable permissions.
- Develop and execute a Bash script.
- Automate repetitive filesystem operations.
- Verify the results of command-line operations.

## Technologies and Tools

- Linux
- Bash
- Linux Terminal
- GNU Core Utilities
- Nano Text Editor

## Prerequisites

- Linux-based operating system such as Ubuntu, Debian, or Fedora
- Bash shell
- Terminal access
- Basic command-line familiarity

## Project Structure

```text
linux-fundamentals-and-bash-automation/
│
├── README.md
├── scripts/
│   └── create_files.sh
├── docs/
│   └── lab-notes.md

| Command    | Purpose                                 |
| ---------- | --------------------------------------- |
| `ls`       | Lists files and directories             |
| `ls -l`    | Displays detailed directory information |
| `ls -a`    | Displays hidden files                   |
| `pwd`      | Displays the current working directory  |
| `cd`       | Changes the current directory           |
| `cd ~`     | Navigates to the home directory         |
| `cd ..`    | Moves to the parent directory           |
| `mkdir`    | Creates a directory                     |
| `rmdir`    | Removes an empty directory              |
| `rm`       | Removes files                           |
| `rm -r`    | Recursively removes directories         |
| `touch`    | Creates an empty file                   |
| `cp`       | Copies files                            |
| `mv`       | Moves or renames files                  |
| `chmod +x` | Grants executable permission            |
| `echo`     | Displays text                           |

Bash Automation
The project includes a Bash script that automates the creation of a directory and multiple files
SCRIPT
#!/bin/bash

# This script creates directories and files
mkdir -p lab_files
cd lab_files
touch file1.txt file2.txt file3.txt
echo "Files created successfully!"

Script Workflow
1. Specifies Bash as the script interpreter
2. Creates the lab-files directory
3. Navigates into the directory
4. Creates three text files
5. Displays a confirmation message
RUNNING THE SCRIPT
Making it executable:
chmod +x scripts/create_files.sh
./scripts/create_files.sh

Expected Result
After execution, the final result should be created:
lab_files/
├── file1.txt
├── file2.txt
└── file3.txt
The terminal should display:
Files created successfully!
Verification
The generated files can be verified with
ls -l lab_files
The current working directory can be checked with:
pwd

Safety Considerations
Commands such as rm and rm -r can permanently remove files and directories.

For practical exercises, destructive commands should only be used on files and directories created specifically for testing.

Learning Outcomes

After completing this project, the learner should be able to:

Navigate a Linux filesystem.
Manage files and directories from the command line.
Understand basic Bash scripting.
Manage executable permissions.
Automate simple filesystem tasks.
Verify command-line operations.
Future Improvements

Future versions of this project may introduce:

File searching with find
Content searching with grep
Advanced permission management
Variables and command-line arguments
Conditional statements
Loops
Input validation
Error handling
More advanced Bash automation
Conclusion

This project establishes a practical foundation in Linux command-line operations and Bash automation. These skills provide a basis for further work in Linux system administration, scripting, automation, and cloud computing.

Author

Muhammad Hamza Siddique

License

This project is intended for educational and learning purposes.

├── screenshots/
│   └── .gitkeep
└── .gitignore
