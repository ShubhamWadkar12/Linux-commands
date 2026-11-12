

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

### System Information

| Command | Description |
|---|---|
| `date` | Displays the current system date and time. |
| `cal` | Displays the calendar. |
| `uname` | Displays basic system information. |
| `uname -a` | Displays all available kernel and system information. |
| `hostname` | Displays the system's hostname. |
| `whoami` | Displays the current logged-in username. |
| `id` | Displays the current user's UID, GID and supplementary groups. |
| `groups` | Displays the groups to which the current user belongs. |
| `history` | Displays previously executed commands. |
| `clear` | Clears the terminal screen. |
| `man command` | Opens the manual page for a command. |
| `command --help` | Displays command usage and available options. |
| `whatis command` | Displays a brief description of a command. |
| `apropos keyword` | Searches manual descriptions for a keyword. |

### File and Directory Management

| Command | Description |
|---|---|
| `touch file.txt` | Creates an empty file or updates its timestamp. |
| `mkdir directory` | Creates a directory. |
| `mkdir -p a/b/c` | Creates parent directories when required. |
| `cp file1 file2` | Copies a file. |
| `cp -r dir1 dir2` | Copies a directory recursively. |
| `mv file1 file2` | Moves or renames a file. |
| `rm file.txt` | Removes a file. |
| `rm -r directory` | Removes a directory and its contents recursively. |
| `rmdir directory` | Removes an empty directory. |
| `cat file.txt` | Displays file contents. |
| `less file.txt` | Views file contents page by page. |
| `more file.txt` | Displays file contents one screen at a time. |
| `head file.txt` | Displays the first 10 lines of a file. |
| `head -n 5 file.txt` | Displays the first 5 lines. |
| `tail file.txt` | Displays the last 10 lines of a file. |
| `tail -n 20 file.txt` | Displays the last 20 lines. |
| `tail -f file.log` | Continuously monitors new log entries. |
| `wc file.txt` | Displays line, word and byte counts. |
| `wc -l file.txt` | Counts the number of lines. |
| `diff file1 file2` | Compares two files line by line. |

### File Searching and Text Processing

| Command | Description |
|---|---|
| `find /path -name "file.txt"` | Searches for a file by name. |
| `find /path -type f` | Finds files only. |
| `find /path -type d` | Finds directories only. |
| `find /path -size +100M` | Finds files larger than 100 MB. |
| `find /path -mtime -7` | Finds files modified within the last 7 days. |
| `grep "error" file.log` | Searches for a specific word or pattern. |
| `grep -i "error" file.log` | Searches without case sensitivity. |
| `grep -r "error" /var/log` | Searches recursively inside directories. |
| `grep -n "error" file.log` | Displays matching lines with line numbers. |
| `grep -v "error" file.log` | Displays lines that do not match. |
| `locate filename` | Searches files using the locate database. |
| `tar -cvf archive.tar directory/` | Creates a tar archive. |
| `tar -xvf archive.tar` | Extracts a tar archive. |
| `tar -czvf archive.tar.gz directory/` | Creates a compressed tar archive. |
| `tar -xzvf archive.tar.gz` | Extracts a gzip-compressed tar archive. |
| `gzip file.txt` | Compresses a file using gzip. |
| `gunzip file.txt.gz` | Decompresses a gzip file. |
| `zip archive.zip file.txt` | Creates a ZIP archive. |
| `unzip archive.zip` | Extracts a ZIP archive. |

### File Permissions and Ownership

| Command | Description |
|---|---|
| `ls -l` | Displays file permissions and ownership. |
| `chmod 755 file.sh` | Sets permissions to `rwxr-xr-x`. |
| `chmod 644 file.txt` | Sets permissions to `rw-r--r--`. |
| `chmod +x script.sh` | Adds execute permission. |
| `chmod u+x file.sh` | Adds execute permission for the owner. |
| `chown user file.txt` | Changes file ownership. |
| `chown user:group file.txt` | Changes file owner and group. |
| `chown -R user:group directory/` | Changes ownership recursively. |
| `chgrp group file.txt` | Changes the group ownership. |
| `umask` | Displays the current file creation mask. |
| `umask 022` | Sets the file creation mask to 022. |
| `getfacl file.txt` | Displays file access control lists (ACLs). |
| `setfacl -m u:username:rw file.txt` | Grants read and write ACL permissions to a user. |
| `setfacl -x u:username file.txt` | Removes a user's ACL entry. |
| `chmod u+s file` | Sets the SUID permission bit. |
| `chmod g+s directory` | Sets the SGID permission bit. |
| `chmod +t directory` | Sets the sticky bit. |

### Users, Groups and Sudo

| Command | Description |
|---|---|
| `whoami` | Displays the current username. |
| `id` | Displays UID, GID and supplementary groups. |
| `groups username` | Displays groups belonging to a user. |
| `sudo -l` | Lists commands the current user can execute with sudo. |
| `sudo useradd username` | Creates a user account. |
| `sudo adduser username` | Creates a user using the interactive adduser utility. |
| `sudo passwd username` | Sets or changes a user's password. |
| `sudo usermod -aG group username` | Adds a user to a supplementary group. |
| `sudo usermod -l newname oldname` | Renames a user account. |
| `sudo userdel username` | Deletes a user account. |
| `sudo userdel -r username` | Deletes a user and their home directory. |
| `sudo groupadd groupname` | Creates a group. |
| `sudo groupmod -n newgroup oldgroup` | Renames a group. |
| `sudo groupdel groupname` | Deletes a group. |
| `sudo passwd -l username` | Locks a user's password. |
| `sudo passwd -u username` | Unlocks a user's password. |
| `cat /etc/passwd` | Displays user account information. |
| `sudo cat /etc/shadow` | Displays protected password hash information. |
| `cat /etc/group` | Displays group information. |
| `sudo visudo` | Safely edits the sudoers configuration. |

### Process, CPU and Memory Management

| Command | Description |
|---|---|
| `ps` | Displays processes associated with the current terminal. |
| `ps aux` | Displays detailed information about running processes. |
| `ps -ef` | Displays processes in full-format listing. |
| `top` | Displays real-time process and resource information. |
| `htop` | Provides an interactive process monitoring interface. |
| `pgrep nginx` | Finds process IDs matching a process name. |
| `pidof nginx` | Displays process IDs for a running program. |
| `kill PID` | Sends the default SIGTERM signal to a process. |
| `kill -9 PID` | Forcefully terminates a process using SIGKILL. |
| `kill -15 PID` | Sends SIGTERM to a process. |
| `pkill nginx` | Sends a signal to processes matching a name. |
| `killall nginx` | Sends a signal to processes named nginx. |
| `nice -n 10 command` | Starts a command with a specified niceness value. |
| `renice 5 -p PID` | Changes the niceness of a running process. |
| `free -h` | Displays RAM and swap usage in human-readable format. |
| `uptime` | Displays system uptime and load averages. |
| `pstree -p` | Displays processes in a tree structure with PIDs. |

### Services and systemd

| Command | Description |
|---|---|
| `systemctl status service` | Displays the status of a service. |
| `sudo systemctl start service` | Starts a service. |
| `sudo systemctl stop service` | Stops a service. |
| `sudo systemctl restart service` | Restarts a service. |
| `sudo systemctl reload service` | Reloads service configuration without a full restart, if supported. |
| `sudo systemctl enable service` | Enables a service at system startup. |
| `sudo systemctl disable service` | Disables automatic startup of a service. |
| `systemctl is-active service` | Checks whether a service is active. |
| `systemctl is-enabled service` | Checks whether a service is enabled. |
| `systemctl list-units --type=service` | Lists loaded service units. |
| `systemctl --failed` | Displays failed systemd units. |
| `systemctl cat service` | Displays a service unit's configuration. |

### Logs and Log Analysis

| Command | Description |
|---|---|
| `ls /var/log` | Lists system log files and directories. |
| `journalctl` | Displays systemd journal logs. |
| `journalctl -xe` | Displays recent journal entries with additional details. |
| `journalctl -u service` | Displays logs for a specific service. |
| `journalctl -f` | Follows new journal entries in real time. |
| `journalctl -u service -f` | Follows logs for a specific service. |
| `tail -f /var/log/syslog` | Continuously monitors the system log. |
| `grep -i error file.log` | Searches logs for errors without case sensitivity. |
| `sudo logrotate -d /etc/logrotate.conf` | Tests logrotate configuration without making changes. |
| `sudo logrotate -f /etc/logrotate.conf` | Forces log rotation. |

### Disk, Storage and Memory

| Command | Description |
|---|---|
| `df -h` | Displays filesystem disk usage in human-readable format. |
| `df -Th` | Displays filesystem types and disk usage. |
| `df -i` | Displays inode usage. |
| `du -sh directory/` | Displays total directory size. |
| `du -ah directory/` | Displays sizes of files and directories. |
| `du -h --max-depth=1 /var` | Displays sizes of immediate subdirectories in `/var`. |
| `lsblk` | Lists block devices and partitions. |
| `lsblk -f` | Displays filesystem information for block devices. |
| `blkid` | Displays block device UUIDs and filesystem types. |
| `sudo fdisk -l` | Lists disk partitions. |
| `mount` | Displays currently mounted filesystems. |
| `sudo mount device mountpoint` | Mounts a filesystem. |
| `sudo umount mountpoint` | Unmounts a filesystem. |
| `cat /etc/fstab` | Displays persistent filesystem mount configuration. |
| `free -h` | Displays RAM and swap usage. |
| `swapon --show` | Displays active swap devices and files. |
| `docker system df` | Displays Docker disk usage. |
| `docker system df -v` | Displays detailed Docker disk usage. |
| `docker info --format '{{.DockerRootDir}}'` | Displays Docker's data directory. |

### Linux Networking

#### Network interfaces and routing

| Command | Description |
|---|---|
| `ip addr` | Displays network interfaces and IP addresses. |
| `ip addr show eth0` | Displays information about the eth0 interface. |
| `ip link` | Displays network interface link information. |
| `ip route` | Displays the kernel IP routing table. |
| `ip route get 8.8.8.8` | Displays the route selected for a destination IP. |

#### Network connectivity

| Command | Description |
|---|---|
| `ping google.com` | Tests network connectivity using ICMP. |
| `ping -c 4 google.com` | Sends four ICMP packets. |
| `traceroute google.com` | Displays the network path to a destination. |
| `ss -tuln` | Displays listening TCP and UDP sockets. |
| `sudo ss -tulnp` | Displays listening sockets with process information. |
| `sudo ss -ltnp 'sport = :80'` | Displays processes listening on TCP port 80. |
| `netstat -tulnp` | Displays listening TCP and UDP ports with process information. |

#### DNS troubleshooting

| Command | Description |
|---|---|
| `nslookup google.com` | Looks up DNS records for a domain. |
| `nslookup -type=A google.com` | Queries IPv4 A records. |
| `nslookup -type=AAAA google.com` | Queries IPv6 AAAA records. |
| `nslookup google.com 8.8.8.8` | Queries a domain using a specified DNS server. |
| `nslookup 8.8.8.8` | Performs a reverse DNS lookup. |
| `dig google.com` | Displays detailed DNS query information. |
| `dig google.com A` | Queries IPv4 A records. |
| `dig google.com AAAA` | Queries IPv6 AAAA records. |
| `dig @8.8.8.8 google.com` | Queries using a specified DNS server. |
| `dig google.com +short` | Displays concise DNS results. |

#### HTTP and HTTPS troubleshooting — curl

| Command | Description |
|---|---|
| `curl https://example.com` | Sends a GET request and displays the response body. |
| `curl -I https://example.com` | Sends a HEAD request and displays response headers. |
| `curl -o /dev/null -s -w "%{http_code}\n" URL` | Displays only the HTTP status code. |
| `curl -L URL` | Follows HTTP redirects. |
| `curl -v URL` | Displays detailed connection, TLS and HTTP debugging information. |
| `curl -X GET URL` | Explicitly specifies the GET method. |
| `curl -X POST URL` | Explicitly specifies the POST method. |
| `curl -H "Accept: application/json" URL` | Sends a custom HTTP header. |
| `curl -H "Authorization: Bearer TOKEN" URL` | Sends a Bearer authorization header. |
| `curl -d '{"key":"value"}' URL` | Sends request data; normally uses POST when no method is specified. |
| `curl --connect-timeout 5 URL` | Sets a 5-second connection establishment timeout. |
| `curl --max-time 10 URL` | Sets a 10-second maximum time for the complete operation. |

#### File downloads — wget

| Command | Description |
|---|---|
| `wget URL` | Downloads a file from a URL. |
| `wget -O filename URL` | Downloads a file using a custom filename. |
| `wget -b URL` | Downloads a file in the background. |
| `wget -o download.log URL` | Saves wget log messages to a specified file. |
| `wget --limit-rate=200k URL` | Limits download speed to approximately 200 KB/s. |
| `wget -c URL` | Attempts to resume an interrupted download. |
| `wget --spider URL` | Checks URL accessibility without retrieving the content. |

---

#### Hostname and DNS troubleshooting

| Command | Description |
|---|---|
| `hostname` | Displays the current system hostname. |
| `hostnamectl` | Displays hostname and system information. |
| `hostname -I` | Displays IP addresses assigned to the system. |
| `cat /etc/hostname` | Displays the configured system hostname. |
| `cat /etc/hosts` | Displays local hostname-to-IP mappings. |
| `cat /etc/nsswitch.conf` | Displays the order of name-service lookup sources. |
| `cat /etc/resolv.conf` | Displays DNS resolver configuration. |
| `resolvectl status` | Displays DNS configuration and status for network interfaces. |
| `getent hosts example.com` | Resolves a hostname using system name-service sources. |
| `getent ahosts example.com` | Displays available address information for a hostname. |
| `getent ahostsv4 example.com` | Resolves IPv4 addresses using system name-service sources. |
| `getent ahostsv6 example.com` | Resolves IPv6 addresses using system name-service sources. |

---

#### Network interface troubleshooting

| Command | Description |
|---|---|
| `ip link show` | Displays network interfaces and their states. |
| `ip link show eth0` | Displays information about the eth0 interface. |
| `ip addr show` | Displays IP addresses assigned to network interfaces. |
| `ip -4 addr` | Displays IPv4 addresses. |
| `ip -6 addr` | Displays IPv6 addresses. |
| `ip -s link show eth0` | Displays RX and TX interface statistics. |
| `cat /sys/class/net/eth0/address` | Displays the MAC address of eth0. |

---

#### Routing table troubleshooting

| Command | Description |
|---|---|
| `ip route` | Displays the IPv4 routing table. |
| `ip route show` | Displays routing information. |
| `ip route get 8.8.8.8` | Shows the route used to reach a destination. |
| `ip -6 route` | Displays the IPv6 routing table. |

---

#### ARP and neighbour table troubleshooting

| Command | Description |
|---|---|
| `ip neigh` | Displays the neighbour table. |
| `ip neigh show` | Displays neighbour entries. |
| `ip -s neigh` | Displays neighbour entries with statistics. |
| `ip -4 neigh show` | Displays IPv4 neighbour entries. |
| `ip -6 neigh show` | Displays IPv6 neighbour entries. |
| `ip neigh show dev eth0` | Displays neighbour entries for eth0. |
| `ip neigh get IP dev eth0` | Displays the neighbour entry for a specific IP. |
| `arp -n` | Displays the ARP table (if installed). |

---
#### Network ports and firewall troubleshooting

| Command | Description |
|---|---|
| `ss -tuln` | Displays listening TCP and UDP ports. |
| `ss -tulnp` | Displays listening ports with process information. |
| `ss -ant` | Displays TCP socket states. |
| `sudo ss -lntup` | Displays listening TCP/UDP sockets and process details. |
| `sudo lsof -i :80` | Identifies processes using port 80. |
| `sudo ufw status` | Displays UFW firewall status. |
| `sudo ufw status verbose` | Displays detailed UFW status. |
| `sudo iptables -L -n -v` | Displays iptables rules and counters. |
| `sudo nft list ruleset` | Displays the nftables ruleset. |
