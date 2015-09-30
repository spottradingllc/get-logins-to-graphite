## Supporting scripts for UnusedServers Module

We distribute these scripts with salt to every server in our environment and then we use information gather by these scripts in UnusedServers module (https://github.com/spottradingllc/unused-servers)

`Logons_To_Graphite.ps1`:  
PowerShell script to send logon informtation from Windows to Graphite. Please modify it according to your needs. This is distributed by salt in our environemnt thus you'll see Jinja templating there. It can easily be modified to PowerShell variables if you cannot use Salt in your environment.

`server_logins_stats`:  
Bash script to send login informtaion from Linux to Graphite. Please modify it according to your needs.
