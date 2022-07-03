# SFS-UPLOADER
Basic server side scripts that handle HTML uploads

HTML component
-----
form has action section which requires a script argument that does the work on server  
this script could be Javascript or PHP or in this case Python

Python component
-----
uploader checks for certain key file names for security  
uploader puts files in misc folder

Bash component
-----
start script near beginning of Python script  
use lsof or something else to check how much has been transfered  
update filename of special status file in misc to show how many megabytes uploaded  
quit Bash script while loop after timeout and write timeout to status  
quit Bash script while loop when Python script signal ends and write complete to status

