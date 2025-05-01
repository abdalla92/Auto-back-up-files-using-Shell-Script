# Automatically back up files using Linux Shell Script

## Scenario

Imagine that you are a lead Linux developer at the top-tech company ABC International Inc. ABC currently suffers from a huge bottleneck: each day, interns must painstakingly access encrypted password files on core servers and back up any files that were updated within the last 24 hours. This process introduces human error, lowers security, and takes an unreasonable amount of work.

As one of ABC Inc.'s most trusted Linux developers, you have been tasked with creating a script called backup.sh, which runs every day and automatically backs up any encrypted password files that have been updated in the past 24 hours.

## Objectives

Demonstrating advanced shell scripting skills in a real-world scenario

## Requirments

[Task 01]: Set two variables equal to the values of the first and second command line arguments, as follows:
              Set targetDirectory to the first command line argument
              Set destinationDirectory to the second command line argument
              
[Task 02]: Display the values of the two command-line arguments in the terminal.

[Task 03]: Define a variable called currentTS as the current timestamp, expressed in seconds.

[Task 04]: Define a variable called backupFileName to store the name of the archived file 
           and a compressed backup file that the script will create

[Task 05]: Define a variable called origAbsPath with the absolute path of the current directory 
           as the variable's value

[Task 06]: Define a variable called destAbsPath whose value equals the absolute path 
           of the destination directory.

[Task 07]: Change directories from the current working directory to the target directory targetDirectory

[Task 08]: Define a numerical variable called yesterdayTS as the timestamp (in seconds) 24 hours prior 
           to the current timestamp, currentTS

[Task 09]: In the for loop, use the wildcard to iterate over all files and directories in the current folder

[Task 10]: Inside the for loop, you want to check whether the $file was modified within the last 24 hours

[Task 11]: In the if-then statement, add the $file that was updated in the past 24 hours to the toBackup array

[Task 12]: After the for loop, compress and archive the files, using the $toBackup array of filenames, 
           to a file with the name backupFileName

[Task 13]: Move the file backupFileName to the destination directory located at destAbsPath

[Task 14]: Submit your completed backup.sh file

[Task 15]: Upload a screenshot showing executable permissions

[Task 16]: Upload screenshot showing file named backup-[TIMESTAMP].tar.gz

[Task 17]: Upload a screenshot showing the crontab schedule of once a day
