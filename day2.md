## Linux For User
1.Information Gathering

Tools for information gathering, in system,network host
like dmitry,ike-scan,legion,maltego,netdiscover,nmap,pof,recon-ng,spiderfoot

2.Vulnerability Analysis

Tools for Finding Vulnerabilities
like legion,lynis,nikto ,nmap

3.Web Application Analysis

Tools for Finding Vulnerabilities and exploits websites -like burpsuite,commix

4.Database Assessment

Tools for Finding Vulnerabilities and exploits on Databases
like sqlmap

5.password Attacks

Tools for exploiting Passwords for login,websites,application, windows..
like Hydra ,cewl,crunch

6.Wireless Attacks

Tools for exploiting Wireless Systems like wiﬁ, bluetooth.. -like aircrack-ng,chirp,reaver

7.Reverse Engineering

Tools for exploiting Softwares, Mobile Applications and any binary ﬁles
like apktool,clang,bytecode-vi

8.Exploitation Tools

Tools for exploiting Softwares, Mobile,Computers ,websites and any things
like armitage,befef xss fra..,

9.Snifﬁng & Spooﬁng

Tools for Listening or hijacking networks
like driftnet,hamster,macchanger

10.POST exploitation

Tools for Maintaining our access. Used after exploiting a system
like nishang,backdoor-f...,powersploit

11.Forensics

Tools for Doing researches and investigate a Cyber Attacks.
like autopsy,binwalk

12.Reporting tools

Tools for Report preparation. After some forensic you will get data and you will write report and these tools will help you.
like sutycapt,pipal

13.Social Engineering tools

Tools Used for Social Engineering attacks
like maltego,beef xss fra...,social engin

14.System Services

Buttons used to start some services.
like beef start,beef stop,dradis start and stop

15.Usually used applications

Softwares for some basic purposes
like accessories,internet,graphics,office,other

## Folder managers

* Dolphin
is KDE's file manager that lets you navigate and browse the contents of your hard drives, USB sticks, SD cards, and more . Creating, moving, or deleting files and folders is simple and fast. Dolphin contains plenty of productivity features that will save you time.

By default, Dolphin uses a global user directory located at ~/Library/Application Support/Dolphin .

* Thunar

Thunar is a modern file manager for the Xfce Desktop Environment. Thunar has been designed from the ground up to be fast and easy-to-use. Its user interface is clean and intuitive, and does not include any confusing or useless options by default. Thunar is fast and responsive with a good start up time and folder load time.

* Nautilus

GNOME Files, formerly and internally known as Nautilus, is the official file manager for the GNOME desktop. Nautilus was originally developed by Eazel with many luminaries from the tech world including Andy Hertzfeld (Apple), chief architect for Nautilus.

## Linux Command Basics

* command

is a program or utility that runs on the CLI – a console that interacts with the system via texts and processes.

Linux commands are executed on Terminal by pressing Enter at the end of the line.

List Directory(ls)

List information about the FILEs (the current directory by default).

ls -l

ls -a

ls filename

ls -R => recursive You can combine them, ls -rla

* Change Directory(cd)

It is used to change current working directory.

cd [directory] ->root

cd / ->home

cd ->1 Back

cd ..

cd ../.. ->2 Back

cd foldername

* pwd

prints the full name (the full path) of current/working directory.

* echo

is used to display line of text/string that are passed as an argument . This is a built in command that is mostly used in shell scripts and batch files to output status text to the screen or a file.
echo text > file.txt

You can add texts(append)

echo text >> ﬁle.txt

## cat / head / tail / less
* cat

print the content of a file onto the standard output stream.

* cat [file]

* head

prints the first lines of one or more files (or piped data) to standard output

* tail
is a command-line utility that displays the last part of file content.

## less

a Linux terminal pager that shows a file's contents one screen at a time.

## touch

a standard program that is used to create, change and modify timestamps of a file.

** touch [file1] [file2]

Creates any kind of Files with the name you gave it. With empty inside.

## Mkdir / make directory

allows users to create or make new directories.

mkdir [FOLDER-NAME1] [FOLDER-NAME2] [FOLDER-NAME3]

## clear

* Clears your screen.

- rm / remove

* removes the entries for a specified file, group of files, or certain select files from a list within a directory.

rm stands for remove

rm [FILE1] [FILE2] [FILE3]

rm -r => recursive(4 folders)

rm -i => for prompt(ask)

rm -f => force delete

ou can use them in combination too like, rm -rf ‘ﬁlename’

## Cp| mv / copy,move

Copy/move ﬁles & folders.

cp [oldFILEplace] [newﬁlePlace]

Mv [oldFILEplace] [newﬁlePlace]

## grep (global search for regular expression)

* The grep filter searches a file for a particular pattern of characters, and displays all lines that contain that pattern. The pattern that is searched in the file is referred to as the regular expression (grep stands for global search for regular expression and print out).

grep [options] pattern [files]

There are a variety of options used along with grep to display the output based on the requirement. A few of these options are:

“-i” – Ignore case sensitivity

“-b” – Display block number at beginning of every line

“-l” – Display file names but not matched lines

“-n” – Display matched lines and line numbers

“-v” – Display lines that do not match

"-c"search ﬁle ,count numbers

"-l" search * displays ﬁlename

"-R" search foldername,search text in folders

## Wc - word count

* It is used to find out number of lines, word count, byte and characters count in the files specified in the file arguments.

wc [OPTION]... [FILE]...

* Multiple Command Executions

### You can run/ execute multiple commands in 1 line using 3 methods:

And ( && )

Or ( || )

Pipeing( | )

AND ( && )

### On AND operation All commands you entered will be executed. If both are working without error
OR ( || )

On OR operation the command will be executed. If it have error or not

Piping ( | )

On pipe, will help you run commands by using the output of the 1st command as the input for the next one.

## What is sed and awk ?

* Sed stands for "stream editor" and it is used to manipulate text by applying a series of commands to each line of a file or input stream. Sed is particularly useful for tasks like searching and replacing text, deleting or adding lines, or performing simple transformations on text.

* Awk, on the other hand, is a powerful text processing tool that allows you to perform complex text manipulation tasks. It is particularly useful for processing structured text, such as data in CSV files or log files. Awk provides a scripting language with a range of built-in functions and operators that make it easy to extract, transform and analyze data.
