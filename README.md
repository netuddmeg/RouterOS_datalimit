### RouterOS_datalimit

RouterOS script for watching/reporting traffic, speed limits, etc.

WHATISIT? (AS I REMEMBER CORRECTLY) 

This script measures the uploaded and downloaded MBs and up/downloading speed on the WAN interface and sends warning if the limit has been reached.

The trigger is alive if:

uploaded MBs OR downloaded MBs
OR
(downloaded data AND uploaded data)
OR
upload speed Mb/s OR download speed Mb/s

...reached (one of) the limit(s).

Maybe I cannot remember well for last 3-4 years, please DONT BE ANGRY if I have mistake this comment.

Define the variables above, and put this script into scheduler!

TESTED and WORKED 100% on RouterOS 6.35.4
This script made in 2015.
This comment added in 2018.

### I WILL NOT DEVELOP THIS STUFF IN THE FUTURE, PLEASE DONT ASK ME! Thanks.

### email recipients
:global emailTo "somebody@xxx.net";
:global emailTo2 "somebody2@xxx.net";
:global emailTo3 "somebody3@xxx.net";
#############################################
### email configuration to send emails (SMPT auth)
:global emailFrom "anotherone@xxx.net";
:global emailSmtp "10.0.0.1";
:global emailPort "25";
:global emailPw "topsecretpassword";
:global emailTls "yes";
:global emailUser "smtpauthuser@xxx.net";
#############################################
### IMPORTANT VARS BEGINING HERE
#############################################
### limitUP/DOWN means MB
:set limitDOWN "200"; 
:set limitUP "270";

### rxtxLIMIT means kbps
:global rxtxLIMIT "500";
