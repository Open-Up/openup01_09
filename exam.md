# Open Up! Mid term exam

You have the right to use internet, but do not communicate with others in the class.

## Unix command (5 pts)

 - Question 1 (2,5 pts): Write a command for modifiying html files of the current directory and its subfolder. You will change 3.0.0-beta5 string into 3.0.0-beta6 string in all these files.


 - Question 2 (2,5 pts): Create a command sum the number of lines of files in the current directory

Example output : 

```
benwa@horizon ~/Documents/linagora/open-up/s01/e08 (git)-[master] % ./script.sh
36
```

Send the commands you wrote by mail to btellier@linagora.com. Specify your name.

## File systems (5 pts)

 - Question 1 (2 pts) : Create a read-only ext4 filesystem on top of a file (you can refer to s01_e07). Use devile /dev/loop0. Mount it in /mnt/ro
 - Question 2 (2 pts) : Create a 128 MB filesystem based on tmpfs. Mount it in /mnt/tmpfs
 - Question 3 (1 pts) : Show the mounted filesystems

Call the instructors for validation.

## Scripting (10 pts)

You will write a script to help me to classify some documents.

We will write here the ./classify.sh script 

 - Question 1 (1 pt) : write a script that creates the folders java and c_plus_plus in the current directory
 - Question 2 (1 pt) : modify the script so that you can run it twice without errors
 - Question 3 (5 pt) : Complete the script. It should move the files containing the word "java" insice the java folder. It should move the files with the world "c_plus_plus" into the c_plus_plus folder.
 - Question 4 (3 pt) : Add a recursive option (-R flag). If present, your script should move files of subdirectoris containing the word "java" into ./java. Same thing for "c_plus_plus"

Send your script by mail to btellier@linagora.com . Specify your name.
