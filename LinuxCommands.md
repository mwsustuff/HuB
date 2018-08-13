__ls__

Shows list of files and directories.

This is probably one of the most commonly typed commands. This has many options to see different types of files and it also supports wild cards.

1.  Show all files in current directory
> ls

2. Show all files in a directory /mydir/some/path
> ls /mydir/some/path

3. Display details of all file in the list 
> ls -l

4.Display all hidden files as well (including the files name start with a do )
> ls -a

5.Display all file that have names starting with my
>ls my*

------------------------------------------------------------------------------------------------------------------------------------

__cd__

Used to change directory

1. Go to the home directory of logged in user
> cd

2. Go to a specific directory named /mydir/some/path
> cd /mydire/some/path

------------------------------------------------------------------------------------------------------------------------------------
__cp__

Copy a file or directory from one location to another. 

1. Copy a file name file1 with name file2
> cp file1 file2

2.Copy the directory name dir1 to dir2
> cp -r dir1 dir2

------------------------------------------------------------------------------------------------------------------------------------
__mkdir__

Create one or more directories

1. Create a directory named mydirecory
> mkdir mydirectory

2. Create 3 directories name dir1, dir2 and dir3
> mkdir dir1 dir2 dir3
------------------------------------------------------------------------------------------------------------------------------------
__man__

_Used to read more details about how to use any command_

There are hundreds of commands and each of these commands are supported with dozens of options. You can always use this command to explore more options supported by a command. 

1. Show help for ls command 
> man ls
2. Show help for grep command 
> man grep
-------------------------------------------------------------------------------------------------------------------------------------
__mv__ - Rename command

_Used for renaming a file or directory. 

Rename file1 to file2

mv file1 file2


System Information
date
The command to see current date or set system date/time
In order to type the date in two digit month formats, two digit time formats, two digit date, two digit minutes, you need this command. This will in changing and setting the date and time over your Linux based computer. This command is very much useful when you want to log on being a root.
Display current date
date
Set current system date to "June 20, 1985, 5:27 PM"

date 0620172785
df
The command for checking available disc space
The computer users are often known to check the availability and consumed memory space over their systems for both the Linux and Windows desktop PCs. You can easily check the amount of memory available over the disk at your Linux system by simply typing the command of DF. It helps in offering you the status of file system disk space over your Linux based system.

df -h
du
Display disk space use by each file in the file system 
Display disk usage by each file in Documents directory
du -h Documents
Display disk usage by the whole Documents direcotry 
du – sh Documents

top
Display the top running processes on the system with memory and cpu utilization. 
Display all top running processes
top
Display all top running processes from user fromdev 
top -U fromdev

ps
Show the status of running processes
Display all running process status for current user
ps
Display the list of all running processes on system with their status.
ps -al

uname 
Find information about version and details of operating system
uname -a


File Operations

gzip
This command will compress a file in gzip format. 

gzip file1


gunzip
Uncompress the gzip file.
gunzip file1.gz


tail
Display last few lines contents of a file. Very useful to watch latest content updates on log file.
Watch running content of a logfile name logfile1 
tail -f logfile1
Display last 100 lines of a file name myfile
tail -100 myfile

scp
Copy a file to or from a remote host
Copy the file "myfile.txt" from a remote host to the local host
scp your_username@remote-server:foobar.txt /path/to/local/directory



Copy a local file myfile.txt to remote server 
scp myfile.txt your_username@remote-server:/path/to/copy/



Copy the directory "mydir" from the local host to a remote host's directory "myremotedir"

scp -r mydir your_username@remote-server:/path/to/remote/directory/myremotedir




sftp
This can be used for doing file transfer using secure ftp protocol. To open a sftp command prompt on a sftp server try this

sftp your_username@remote-server


cat
Used to display the content of the file on console without opening it in a editor.. 
cat myfile

more 
Used to display the content of a file on console with option to navigate in case the content is too large to fit in screen.
more myfile


find
Find a file or directory on the system using this command
Find a file myfile.txt in current directory and its subdirectories. 
find . -name “myfile.txt”
Find all files in Documents directory that are larger that 25MB in size
find . -size +25M -exec du -h {} \;
Find all .doc files on the system that have been modified in the last 5 days.
find . –name “*.doc” –mtime -5
Find all .txt files on the system that were modified in last 15 minutes
find . –name “*.txt” –mmin -15
Find all files that contain a string “I am inside file”.
find . -name "*" -exec grep -i -H "I am inside file" {} \;

grep
This command is used to search all the lines in all files in a specified location containing a string. 
Search for a specific string “myname” in a file myfile.txt
grep “myname” myfile.txt
Search for a specific string “myname” with ignoring the case in a file myfile.txt
grep -i “myname” myfile.txt
Search for a specific string “myname” in a all files in current directory
grep “myname” *
Search for full word “myword” in a file myfile.txt
grep -w “myword” myfile.txt
Search a string “myname” in all files in all subdirectories recursively 
grep -r “myname” *

rm 
Remove a file or directory using this command

Remove a file name myfile.txt 
rm myfile.txt



Remove a directory mydir 
rm -r mydir



Remove a file myfile.txt forcefully
rm -f myfile.txt




* __chmod__

The command for manipulating the file permissions

For better security, the permissions for file in Linux OS are categorized into different groups, users and other sections. You have the option of controlling the permissions by assigning the users under the given divisions via the command of ‘chmod’. These permissions would help the users to write, read and execute the respective files. This option is very much handy when you have to run a script in order to install the package, which remains non executable in the default for security reasons. With the command of ‘chmod +x’ you could end up making the script executable over your Linux system.

Provide execute permission on a file myfile.txt to all users
> chmod +x myfile.txt

Provide read permission on a file myfile.txt to all users
> chmod +r myfile.txt

Provide full permissions (read/write/execute) on a file myfile.txt to yourself but everyone else has only read and execute
> chmod 755 myfile.txt

Provide full permissions (read/write/execute) on a file myfile.txt to everyone
> chmod 777 myfile.txt

chown 
Change ownership of a file. You should be either root or the owner of the file to successfully run this command. 
Change the ownership of a file myfile.txt to another_user who is part of another_group

chown another_user:another_group myfile.txt




Change the ownership of a directory mydir1 recursively to another_user who is part of another_group

chown -R another_user:another_group mydir1



Other Useful Commands

passwd 
This is the command for changing the password. Passwords play an important role in securing your data found in your desktop computer. In order to keep the system full proof against the hacking attacks, you need to keep on changing your passwords every three months. The users over Linux computers could do the same using a particular command of ‘change password’ over the command prompt and do the needful. After you type the command, all you need to do is to type the new password twice, and you are done with the same.


logout
Command for logging out. By typing this command, you would be logged out from your Linux based computer. This command will help in disconnecting from your Linux based PCs or simply help in logging out the session that you are seen over your desktop. All you need to do is to remember the account you have logged out as it may bring a couple of security issues. Hence it is highly suggested to use a log out the moment you finish your task over your PC.


kill -9
The command to terminate the process by its process id. You may find certain Linux applications not responding at such junctures, you could simply get away from this scenario by typing the kill command, which will help in terminating the process. For this you need the process ‘PID’ of the particular application, which could be done with the help of “ps” command. You could further use this command to kill the command to terminate the application, which is not responding.

Terminate a process with with ID 1234

kill -9 1234

”>” - The operator to redirect output
Though this may not be called as a command by many yet it is among the important steps to master while you start working with Linux over the command line. For this you need several tools, which also include the pipe. These help in redirecting the output (that is often printed over the screen) somewhere else like the text file or any other application. This command is used to complete any file over the Linux system.
Copy content of file1 to file2
cat file1 > file2
Append content of file1 to file2
cat file1>>file2
Create a new file myfile.txt with text “some text” 
echo “some text” > myfile.txt

__pipe (|) operator__
The pipe operator is a powerful operator that can be used to join two commands together. Usign this operator output of one command can become input to another command. For example


Display live occurrence of text “myname” in a file myfile.log
> tail -f myfile.logs | grep “myname”


* Count the number of lines in a file myfile1 
> cat myfile1 | wc -l

* Find all running java processes on a system
> ps -aef | grep “java”

* Find all .txt files containing text “myname” 
> find . -name “*.txt” | xargs grep “myname”

* __history__

This is the command for recall. 

You need to use history to rerun any command. If you enter this command without any kind of switch, you end up getting the history list along with the line numbers. Also, you could even perform some additional search of the given history list with this command.


* __exit__
Use this to quit the command line shell on a linux system.
