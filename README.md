<h1>Scripting for Compression and Backup</h1>

<h2>Description</h2>
Project consists of building a safety plan for a directory by writing an automated script that compresses/backs up the folder.
<br />


<h2>Utilities Used</h2>

- <b>VirtualBox</b>
- <b>Debian Environment</b>
- <b>Terminal</b>
- <b>Tar</b>


<h2>Writing a Bash Script for Data Backup:</h2>
A script will be set to generate a daily copy of all files and subfolder's within a user's home directory. The script will compress the /home/ directory and save the compressed file to the /tmp folder. The status of each step will be printed to ensure proper function.
<br />
<br />
A file named backupScript.sh is created with nano:<br/>
<img src="https://imagizer.imageshack.com/img922/8346/UEd29i.png"
<br />
<br />
The script is began by defining the home directory as a variable called backup_files:<br/>
<img src="https://imagizer.imageshack.com/img922/9461/t4xebf.png"
<br />
<br />
A variable named dest is created and points to the /tmp directory:<br/>
<img src="https://imagizer.imageshack.com/img924/7665/AOipGv.png"
<br />
<br />
A varaible named now is created that will contain the start and end times of the script when it is run as an executable:<br/>
<img src="https://imagizer.imageshack.com/img924/3158/qIlS48.png"
<br />
<br />
Three variables are created. One to specify the date that the backup was created, one to include the hostname, and one more to combine both variables into an archive file:<br/>
<img src="https://imagizer.imageshack.com/img923/7281/vWuE6D.png"
<br />
<br />
Two echo commands are executed to show which directory is being backed up, where the backup will be saved, and that the process is starting:<br/>
<img src="https://imagizer.imageshack.com/img922/1235/LBLerf.png"
<br />
<br />
Another echo is included to print the script start time:<br/>
<img src="https://imagizer.imageshack.com/img924/8831/pNtjv1.png"
<br />
<br />
The tar command is written including the two previously defined varibales. This line will compress the /home/ directory to the /tmp directory:<br/>
<img src="https://imagizer.imageshack.com/img922/3484/nk6lBl.png"
<br />
<br />
A message is written to print the script's completion status and end time:<br/>
<img src="https://imagizer.imageshack.com/img922/7481/vMcYq3.png"
<br />
<br />
The script is saved and made executable:<br/>
<img src="https://imagizer.imageshack.com/img924/9684/ezTNHm.png"
<br />
<br />
The script is executed- the echo messages can be seen:<br/>
<img src="https://imagizer.imageshack.com/img924/7284/qH3szp.png"
<br />
<br />
The .tgz backup file is confirmed in the /tmp directory:<br/>
<img src="https://imagizer.imageshack.com/img924/8940/Sy0cTu.png"
<br />
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
