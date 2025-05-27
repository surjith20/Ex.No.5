# 19CS545-Ex5 - Set a Cron job in GitHub

# AIM:
To set a Cron job.

# Procedure:
1. Edi ng crontab 
The first line [root@servera:~]# crontab -e harry edits the crontab for the user 
harry. The crontab command is used to manage cron jobs for users. The -e op on specifies 
that the user's crontab file should be opened in a text editor. In this case, since the user execu ng 
the command is root (the system administrator), they are able to edit the crontab for another 
user (harry). 
2. Adding a cron job 
The line 30 12 * * * /bin/bash /home/harry/backup.sh is most likely the line 
that was added to the crontab file. This line defines a new cron job. 
Cron jobs use a specific format to define the schedule and command to be executed. The format is: 
minute hour day of month month day of week command 
Each field is separated by a space and defines a specific value or range of values. An asterisk (*) in 
any field represents "all possible values" for that field. 
In this case, the cron job is defined as follows: 
• Minute: 30 - This means the job will run at the 30th minute of every hour. 
• Hour: 12 - This means the job will run at 12 o'clock. 
• Day of month: * - This wildcard symbol indicates that the job will run on every day of the 
month. 
• Month: * - This wildcard symbol indicates that the job will run in every month of the year. 
• Day of week: * - This wildcard symbol indicates that the job will run on every day of the 
week (Monday through Sunday). 
• Command: /bin/bash /home/harry/backup.sh - This specifies the command to 
be executed. The /bin/bash part tells the system to use the Bash shell to execute the 
script. The /home/harry/backup.sh part specifies the path to the script that will be 
run. 
3. Saving the crontab 
10
A er edi ng the crontab file, the user would typically save and exit the text editor. Since we don't 
see the specific commands used to save the file, I can't say for sure how this was done in this 
instance. 
In summary, these commands set up a cron job to run a script named /home/harry/
 backup.sh at 12:30 every day. The script itself is not shown in the image so it is impossible to 
know what the script does.

# Output:
![image](https://github.com/user-attachments/assets/91e2402f-b51e-4175-94ca-7f79c84297e6)

# Result:
Thus a cron job has been set successfully for the user harry.. 
