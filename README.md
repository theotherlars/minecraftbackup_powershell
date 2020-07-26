# minecraftbackup_powershell
Backup your minecraft server with powershell

Required changes to the script:
  - location of the server folder
  - location of the backup folder
 
Optional changes to the script:
  - $daysToKeepBackup, change this variable to how many days you want to keep the backup before the script deletes it. 

FOR SCHEDULED BACKUP
Add this script to the task scheduler on your windows minecraft server
Under action you type:
  "C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe"  -ExecutionPolicy Bypass "minecraftbackup.ps1 file location" 
