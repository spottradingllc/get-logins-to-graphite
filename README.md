## Supporting scripts for UnusedServers Module

We distribute these scripts with salt to every server in our environment and then we use information gathered by these scripts in UnusedServers module (https://github.com/spottradingllc/unused-servers)

`Logons_To_Graphite.ps1`:  
PowerShell script to send logon information from Windows to Graphite. Please modify it according to your needs. This is distributed by salt in our environment thus you'll see Jinja templating there. It can easily be modified to PowerShell variables if you cannot use Salt in your environment. _This script requires Spot-Graphite PowerShell module._

`server_logins_stats`:  
Bash script to send login information from Linux to Graphite. Please modify it according to your needs.

The scripts are scheduled to run every hour and collect information on how many users logged in locally to the server.
