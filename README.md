DavidDebloater 0.6.0-beta

-App description:
A WPF-based, lightweight solution designed to manage Windows AppX packages and preinstalled bloatware. It also features a scheduling system to periodically check on your user account to remove reappearing bloatware.

!!Warning!! Beta release: This software modifies system packages and Windows Registry entries. It is provided as-is. Please create a System Restore point before using it.
This tool is intended for advanced users and IT professionals. The author is not responsible for any system instability or data loss caused by removing essential Windows packages.

-Prerequisites:
#Windows 10 or Windows 11
#.NET Desktop Runtime 8.0
#Administrator Privileges

-Features:
#Install and uninstall selected AppX packages
#Scheduled removal (Repeated Debloating Tool)
#Security levels: Apps are categorized into security levels:
>Light: Basic bloatware and third-party apps. Safe to remove
>Heavy: Includes built-in Windows telemetry apps and non-critical tools
>Extreme: Aggressive removal. May break core Windows features
>Unfiltered: No filter on the AppX packages except for those which can damage the installation process
#The categories are contained in a whitelist. There is a hash-based compromise detection on the file. If the whitelist gets modified, it alerts on the main menu, but doesn't block any features
#The Extreme and Unfiltered modes have a password protection to avoid accidental deletion of certain packages. The password is 3141

-Known issues and limitations:
#This version allows single-user debloating only (multi-user support is in developement)
#Some apps remain unremoveable due to Windows limitations (Not yet overriden)
#This application only removes the installed bloatware but does not delete the installers in the provisioned storage

-Features already in developement:
#Multi-user bloatware removal and restore
#Provisioned storage cleanup and permanent system-wide removal
#Expanded scheduling configurations for repeated bloatware removal tasks
#Dynamic override mechanisms for built-in AppX protection locks

