# **Linux Commands Cheat Sheet**

Useful GNU/Linux cli commands

The following list of commands are the basic ones. The below table shows the **command**, **category** and **description**.

The **category** column is based on the are where the command is useful for.

&nbsp;

## **Commands List Table**

| command                           | category                                      | description
|---                                |---                                            |---
| cd                                | Navigation                                    | Go to the $HOME directory
| cd ..                             | Navigation                                    | To go up one level of the directory tree
| cd /dir                           | Navigation                                    | Change to /dir directory
| uname -a                          | System                                        | Display Linux system information
| uname -r                          | System                                        | Display kernel release information
| uptime                            | System                                        | Show the period of time the system has been running
| hostname                          | System                                        | Show system hostname
| hostname -I                       | System                                        | Display host IP address
| last reboot                       | System                                        | Show system reboot history
| date                              | System                                        | Show the current date and time
| cal                               | System                                        | Shows current month calendar
| w                                 | System, User Info and Management              | Show users online
| who                               | System, User Info and Management              | Show users online and shows user activity
| whoami                            | System                                        | Shw who you are logged in as
| dmesg                             | Hardware                                      | Review and monitor hardware device and driver messages from the kernel’s own ring buffer
| cat /proc/cpuinfo                 | Hardware                                      | Displays CPU information
| cat /proc/meminfo                 | Hardware                                      | Displays RAM information
| free -h                           | Hardware, Monitoring and Statistics           | Display free and used RAM (-h = human readable, -m = MB, -g = GB)
| lspci -tv                         | Hardware                                      | Display PCI devices
| lsusb -tv                         | Hardware                                      | Display USB devices
| dmidecode                         | Hardware                                      | Display DMI/SMBIOS (hardware info) from the BIOS
| hdparm -i /dev/sda                | Hardware                                      | Show disk sda information
| hdparm -tT /dev/sda               | Hardware                                      | Perform a read speed test on disk sda
| badblocks -s /dev/sda             | Hardware                                      | Test for unreadable blocks on disk sda
| top                               | Monitoring and Statistics, Process Management | Display and manage the top processes
| htop                              | Monitoring and Statistics, Process Management | Interactive process viewer (top alternative)
| mpstat 1                          | Monitoring and Statistics                     | Display processor related statistics
| vmstat 1                          | Monitoring and Statistics                     | Display virtual memory statistics
| iostat 1                          | Monitoring and Statistics                     | Display I/O statistics
| tail 100 /var/log/messages        | Monitoring and Statistics                     | Display the last 100 syslog messages (Use /var/log/syslog​ for Debian based systems.)
| tcpdump -i eth0                   | Monitoring and Statistics                     | Capture and display all packets on interface eth0
| tcpdump -i eth0 'port 80'         | Monitoring and Statistics                     | Monitor all traffic on port 80 ( HTTP )
| lsof                              | Monitoring and Statistics                     | List all open files on the system
| lsof -u user                      | Monitoring and Statistics                     | List files opened by user
| watch df -h                       | Monitoring and Statistics                     | Execute "df -h", showing periodic updates
| id                                | User Info and Management                      | Display the user and group ids of your current user
| last                              | User Info and Management                      | Display the last users who have logged onto the system
| groupadd test                     | User Info and Management                      | Create a group named "test"
| useradd -c "Full Name" -m john    | User Info and Management                      | Create an account named john, with a comment of "John Smith" and create the user's home directory
| userdel john                      | User Info and Management                      | Delete the john account
| usermod -aG sales john            | User Info and Management                      | Add the john account to the sales group
| ls -al                            | Files and Directories                         | List all files in a long listing (detailed) format
| pwd                               | Files and Directories                         | Display the present working directory
| mkdir DirName                     | Files and Directories                         | Creates a directory
| rm file                           | Files and Directories                         | Deletes a file
| rm -r directory                   | Files and Directories                         | Deletes a directory (recursively)
| rm -f file                        | Files and Directories                         | Force deletion of a file without prompting for confirmation
| rm -rf directory                  | Files and Directories                         | Force deletion of a directory without prompting for confirmation
| cp file1 file2                    | Files and Directories                         | Copy file1 to file2
| cp -r source_dir destination      | Files and Directories                         | Copy source_dir​ recursively to destination​ (It creates destination if does not exist)
| mv file1 file2                    | Files and Directories                         | Rename or move file1​ to ​file2 (If exists it will rename it)
| ln -s /path/to/file linkname      | Files and Directories                         | Creates symbolic link to ​linkname
| touch file                        | Files and Directories                         | Creates an empty file
| cat file                          | Files and Directories                         | View the contents of ​file
| less file                         | Files and Directories                         | Browse through a text file
| head file                         | Files and Directories                         | Display the first 10 lines of file
| tail file                         | Files and Directories                         | Display the last 10 lines of file
| tail -f file                      | Files and Directories                         | Display the last 10 lines of file​ and "follow" the file as it grows
| ps                                | Process Management                            | Display your currently running processes
| ps -ef                            | Process Management                            | Display all current running processes
| kill pid                          | Process Management                            | Kill process with process ID of pid
| killall processname               | Process Management                            | Kill all processes named processname
| programname &                     | Process Management                            | & after the programname, starts a program in the background
| bg                                | Process Management                            | Display stopped or background jobs
| fg                                | Process Management                            | Brings the most recent background job to foreground
| fg bgjob                          | Process Management                            | Brings bgjob to foreground
| ifconfig -a / ip a                | Networking                                    | Display all network interfaces and ip address
| ifconfig eth0                     | Networking                                    | Display eth0 address and details
| ethtool eth0                      | Networking                                    | Query or control network driver and hardware settings
| ping host                         | Networking                                    | Send ICMP echo request to host
| whois domain                      | Networking                                    | Display whois information for domain
| dig domain                        | Networking                                    | Display DNS information for domain
| dig -x IP_ADDRESS                 | Networking                                    | Reverse lookup of IP_ADDRESS
| host domain                       | Networking                                    | Display DNS ip address for domain
| hostname -i                       | Networking                                    | Display the network address of the host name
| hostname -I                       | Networking                                    | Display all local ip addresses
| wget domain.com/file              | Networking                                    | Download domain.com/file
| netstat -nutlp                    | Networking                                    | Display listening tcp and udp ports and corresponding programs
| nslookup                          | Networking                                    | TOODO
| tar cf archive.tar directory      | Networking                                    | Create tar named archive.tar containing directory
| tar xf archive.tar                | Networking                                    | Extract the contents from archive.tar
| tar czf archive.tar.gz directory  | Networking                                    | Create a gzip compressed tar file name archive.tar.gz
| tar cjf archive.tar.bz2 directory | Networking                                    | Create a tar file with bzip2 compression
| tar xjf archive.tar.bz2           | Networking                                    | Extract a bzip2 compressed tar file
| tar zxvf sourcecode.tar.gz<br>cd sourcecode<br>./configure<br>make<br>make install | Networking | Install software from source code
| grep pattern file                 | Search                                        | Search for pattern in file
| grep -r pattern directory         | Search                                        | Search recursively for pattern in directory
| locate name                       | Search                                        | Find files and directories by name
| find /home/john -name 'prefix*'   | Search                                        | Find files in /home/john that start with "prefix"
| find /home -size +100M            | Search                                        | Find files larger than 100MB in /home
| ssh host                          | SSH                                           | Connect to host as your local username
| ssh user@host                     | SSH                                           | Connect to host as user
| ssh -p port user@host             | SSH                                           | Connect to host using port
| scp file.txt server:/tmp          | File Transfer                                 | Secure copy file.txt to the /tmp folder on server
| scp server:/var/www/*.html /tmp   | File Transfer                                 | Copy *.html files from server to the local /tmp folder
| scp -r server:/var/www /tmp       | File Transfer                                 | Copy all files and directories recursively from server to the /tmp folder
| rsync -a /home /backups/          | File Transfer                                 | Synchronize /home to /backups/home
| rsync -avz /home server:/backups/ | File Transfer                                 | Synchronize files/directories between the local and remote system with compression enabled
| df -h                             | Disk/s                                        | Show free and used space on mounted filesystems
| df -i                             | Disk/s                                        | Show free and used inodes on mounted filesystems
| fdisk -l                          | Disk/s                                        | Display disks partitions sizes and types
| du -ah                            | Disk/s                                        | Display disk usage for all files and directories in human readable format
| du -sh                            | Disk/s                                        | Display total disk usage off the current directory


&nbsp;

## **Permissions**

![](/%40assets/permissions.png)

| <sup><sup><sup>(octal repreentation)</sup></sup></sup><br>number   | <br>reference | <br>description
|---                                                                            |---            |---
| 0                                                                             | ---           | No permission
| 1                                                                             | --x           | Execute
| 2                                                                             | -w-           | Write 
| 3                                                                             | -wx           | Write + Execute
| 4                                                                             | r--           | Read
| 5                                                                             | r-x           | Read + Execute
| 6                                                                             | rw-           | Read + Write
| 7                                                                             | rwx           | Read + Write + Execute

&nbsp;

### **Symbolic Mode (chmod)**

| operator  | description
|---        |---
| +         | Adds Permission
| -         | Removes Permission
| =         | Sets permissions and overrrides the permissions set previously

&nbsp;

| <sup>(denotations)</sup><br>owners    | <br>target
|---                                    |---
| u                                     | user/owner
| g                                     | group
| o                                     | other
| a                                     | all

&nbsp;

#### **Reference Table**

| <sup>(user)</sup><br>U    | <sup>(group)</sup><br>G   | <sup>(other/world)</sup><br>O | <sup>(number)</sup><br>chmod  | <sup>(reference)</sup><br>chmod   | <br>description
|---                        |---                        |---                            |---                            |---                                |--
| rwx                       | rwx                       | rwx                       | chmod 777 filename | chmod a=rwx filename  | User = Read + Write + Execute<br>Group = Read + Write + Execute<br>Other = Read + Write + Execute<br>
| rwx                       | rwx                       | r-x                       | chmod 775 filename | chmod o-w filename  | User = Read + Write + Execute<br>Group = Read + Write + Execute<br>Other = Read + Execute<br>
| rw-                       | r--                       | r--                       | chmod 644 filename | chmod a=r,u+w  filename  | User = Read + Write<br>Group = Read<br>Other = Read<br>