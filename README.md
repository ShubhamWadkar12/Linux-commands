# Linux Administration

## Table of Contents

1. [Linux Basics and System Information](#1-linux-basics-and-system-information)
2. [Linux Architecture](#2-linux-architecture)
3. [Terminal and Shell](#3-terminal-and-shell)
4. [CLI and GUI](#4-cli-and-gui)
5. [Linux Boot Process](#5-linux-boot-process)
6. [Linux Command Syntax](#6-linux-command-syntax)
7. [Getting Help in Linux](#7-getting-help-in-linux)
8. [Basic Linux Commands](#8-basic-linux-commands)

---

## 1. Linux Basics and System Information

| Command | Explanation |
|---|---|
| `cat /etc/os-release` | Displays Linux distribution name, version and release information. |
| `uname -s` | Displays the operating system kernel name. |
| `uname -r` | Displays the Linux kernel release version. |
| `uname -a` | Displays detailed kernel and system information. |

## 2. Linux Architecture

| Command | Explanation |
|---|---|
| `lscpu` | Displays CPU architecture, processor details and hardware information. |
| `uname -a` | Displays kernel and machine architecture information. |

## 3. Terminal and Shell

| Command | Explanation |
|---|---|
| `echo $SHELL` | Displays the path of the user's configured login shell. |
| `ps -p $$` | Displays information about the currently running shell process. |
| `which bash` | Displays the location of the Bash executable. |

## 4. CLI and GUI

| Command | Explanation |
|---|---|
| `pwd` | Displays the current working directory. |
| `whoami` | Displays the username of the current user. |
| `date` | Displays the current system date and time. |
| `hostname` | Displays the system hostname. |
| `clear` | Clears the visible terminal screen without deleting command history. |

## 5. Linux Boot Process

| Command | Explanation |
|---|---|
| `ps -p 1 -o pid,comm,args` | Displays PID 1, its command name and command-line arguments. |
| `uptime` | Displays system running time and load averages. |
| `systemd --version` | Displays the installed systemd version. |
| `who -b` | Displays the last system boot time, if available. |
| `dmesg` | Displays kernel ring-buffer messages, useful for hardware and kernel troubleshooting. |
| `dmesg \| head -20` | Displays the first 20 lines of kernel messages. |

## 6. Linux Command Syntax

### General Command Syntax

```bash
command [options] [arguments]
```

Examples:

| Command | Explanation |
|---|---|
| `ls -l` | Lists directory contents in detailed format. |
| `ls -a` | Lists all entries, including hidden files. |
| `ls -lh` | Displays directory contents in detailed format with human-readable sizes. |
| `ls -lah` | Lists all entries in detailed format with human-readable sizes. |
| `ls --all` | Displays all directory entries, including hidden files. |
| `ls /etc` | Lists the contents of the `/etc` directory. |
| `ls -lah /var/log` | Lists all entries in `/var/log` with detailed, human-readable information. |
| `mkdir devops` | Creates a directory named `devops`. |
| `mkdir "devops training"` | Creates a directory whose name contains a space. |
| `cat /etc/os-release` | Displays the contents of the OS release information file. |

## 7. Getting Help in Linux

| Command | Explanation |
|---|---|
| `ls --help` | Displays quick usage information and available options for `ls`. |
| `mkdir --help` | Displays help information and available options for `mkdir`. |
| `man ls` | Opens the detailed manual page for the `ls` command. |
| `man 1 ls` | Opens section 1 documentation for the `ls` user command. |
| `man 5 passwd` | Opens documentation for the `/etc/passwd` file format. |
| `whatis ls` | Displays a one-line description of the `ls` command. |
| `whatis systemctl` | Displays a one-line description of the `systemctl` command. |
| `apropos password` | Searches manual-page names and descriptions for password-related topics. |
| `apropos directory` | Searches manual-page names and descriptions for directory-related topics. |

### Useful Manual Page Navigation Keys

| Key | Explanation |
|---|---|
| `Space` | Moves forward one page. |
| `b` | Moves backward one page. |
| `/word` | Searches for a word in the manual page. |
| `n` | Moves to the next search match. |
| `q` | Exits the manual page. |

## 8. Basic Linux Commands

### Date and Time

| Command | Explanation |
|---|---|
| `date` | Displays the current system date and time. |
| `date "+%Y-%m-%d"` | Displays the date in year-month-day format. |
| `date "+%H:%M:%S"` | Displays the current time in 24-hour format. |
| `date "+%A"` | Displays the full weekday name. |
| `date "+%Y-%m-%d %H:%M:%S"` | Displays date and time in a structured format. |

### Calendar

| Command | Explanation |
|---|---|
| `cal` | Displays the current month's calendar. |
| `cal 11 2026` | Displays the calendar for November 2026. |
| `cal 2026` | Displays the complete calendar for 2026. |

### Terminal Management

| Command | Explanation |
|---|---|
| `clear` | Clears the visible terminal screen. |

### Command History

| Command | Explanation |
|---|---|
| `history` | Displays previously executed shell commands. |
| `history 10` | Displays the last 10 commands in shell history. |
| `history \| grep docker` | Searches command history for commands containing the word `docker`. |

### System Information

| Command | Explanation |
|---|---|
| `uname` | Displays the kernel name. |
| `uname -s` | Displays the kernel name explicitly. |
| `uname -r` | Displays the kernel release version. |
| `uname -v` | Displays kernel version and build information. |
| `uname -m` | Displays machine hardware architecture. |
| `uname -n` | Displays the network node hostname. |
| `uname -a` | Displays all available basic system information. |
| `hostname` | Displays the system hostname. |
| `hostnamectl` | Displays hostname and related system information on supported systemd systems. |

---

## Important Linux Command Differences

| Command | What it tells you |
|---|---|
| `uname -r` | Linux kernel release version. |
| `hostname` | Name assigned to the system. |
| `cat /etc/os-release` | Linux distribution and version. |
| `whoami` | Current username. |
| `pwd` | Current working directory. |
| `uptime` | System uptime and load averages. |
| `history` | Previously entered shell commands. |


### Linux Filesystem and Directory Navigation

| Command | What it tells you |
|---|---|
| `ls` | Lists files and directories in the current location. |
| `ls -l` | Displays files with detailed information, including permissions, ownership and size. |
| `ls -a` | Displays all entries, including hidden files and directories. |
| `ls -lh` | Displays file details with human-readable sizes. |
| `ls -lah` | Displays all entries, including hidden ones, with detailed information and human-readable sizes. |
| `ls /var/log` | Lists the contents of the system log directory. |
| `ls -la` | Displays all entries with detailed information. |
| `ls -l ~/.bashrc` | Displays detailed information about the user's Bash configuration file. |
| `head -20 ~/.bashrc` | Displays the first 20 lines of the Bash configuration file. |
| `cd /` | Changes the current directory to the filesystem root. |
| `cd ~` | Changes the current directory to the current user's home directory. |
| `cd` | Takes the user to their home directory. |
| `cd ..` | Moves one level up to the parent directory. |
| `cd ../..` | Moves two directory levels up. |
| `cd -` | Switches to the previous working directory. |
| `cd /etc` | Navigates directly to the `/etc` directory. |
| `cd /var/log` | Navigates directly to the system log directory. |
| `cd Documents` | Navigates to a directory named Documents relative to the current location. |
| `cd projects` | Navigates to the projects directory relative to the current location. |
| `cd ../documents` | Navigates to the documents directory in the parent directory, if it exists. |
| `cd ./projects` | Navigates to the projects directory relative to the current directory. |
| `tree` | Displays files and directories in a hierarchical tree structure. |
| `tree -L 1` | Displays the directory tree up to one level. |
| `tree -L 2` | Displays the directory tree up to two levels. |
| `tree -d` | Displays directories only. |
| `tree -a` | Includes hidden files and directories in the tree. |
| `tree -h` | Displays file sizes in human-readable format. |
| `tree /var/log` | Displays the directory tree of `/var/log`. |
| `tree -d -L 2` | Displays directories only, up to two levels deep. |
| `tree -a -L 2` | Displays all entries, including hidden ones, up to two levels deep. |

**Path symbols:**

| Symbol | Meaning |
|---|---|
| `/` | Filesystem root directory. |
| `~` | Current user's home directory. |
| `.` | Current directory. |
| `..` | Parent directory. |
| `-` | Previous working directory when used with `cd`. |

---


**My learning rule:** Every new Linux command will be added to this README under its respective topic, along with a concise explanation and practical learning status.
# Linux-commands
