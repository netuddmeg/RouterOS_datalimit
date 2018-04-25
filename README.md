### RouterOS_datalimit

RouterOS script for watching/reporting traffic, speed limits, etc.

WHATISIT? (AS I REMEMBER CORRECTLY) 

This script measure the uploaded and downloaded MBs and up/downloading speed on the WAN interface and send warning if the limit has been reached.

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
