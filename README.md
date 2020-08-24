# minecraftbackup_powershell
Backup your minecraft server with powershell.
This script archives the Mincraft "world" folder (.zip) and moves it to a backup folder/location.
It also deletes the oldest .zip based on the $daysToKeepBackup variable

### Required changes to the script
  - location of the server folder
  - location of the backup folder
 
### Optional changes to the script
  - $daysToKeepBackup, change this variable to how many days you want to keep the backup before the script deletes it. 

### Schedule for backup
Add this script to the Task Scheduler on your Windows machine that runs either the Minecraft client or server.  
  
  Under action when you create the task:
```
"C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe"  -ExecutionPolicy Bypass "minecraftbackup.ps1 file location" 
```
