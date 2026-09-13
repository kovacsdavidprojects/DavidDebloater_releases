DavidDebloater 0.9.0-beta

-App description:
A WPF-based, lightweight solution designed to manage Windows AppX packages and preinstalled bloatware. It also features a scheduling system to periodically check on your user account to remove reappearing bloatware.

!!Warning!! Beta release: This software modifies system packages and Windows Registry entries. It is provided as-is. Please create a System Restore point before using it.
This tool is intended for advanced users and IT professionals. The author is not responsible for any system instability or data loss caused by removing essential Windows packages.

-Prerequisites:
--Windows 10 or Windows 11
--.NET Desktop Runtime 8.0
--Administrator Privileges

-CHANGELOG:
--Added "all users" mode to Remove, Restore and Scheduler sections
--Sick new design
--You can remove provisioned packages from now on
--Updated scheduler settings
--Minor bug fixes and improvements
--Refined the filters to hide unremoveable apps

Password to unlock certain features: 3141

-How to use?
--AppX Remover: The list contains installed AppX packages. By selecting the elements on the list manually or using the select/deselect all buttons, then clicking on Remove Selected, you can start the removal process.
---'All users' mode: By enabling all-users mode, you can switch the list to display AppX packages installed for any users on the computer except for System and Guest.
---By clicking on Remove Selected with 'All users' mode active, the removal process will set Active Setup up for every single user. Active Setup will be triggered at their next login removing the selected apps.
--AppX Recover: The list contains every single AppX packages that were removed by DavidDebloater. All users mode exists here as well, making a difference between single and multi-user debloats.
---If provisioned packages were removed for a specific package, there will be a comment about the situation. You can't recover these apps.
--Scheduler: Select packages for removal and set up how often would you like the process to run. By ticking "Remove for all users" the process will use Active Setup and will take effect on the next login.
--Permanent Package Removal: Enables removal of Provisioned Packages. You can't recover these apps anymore without the provisional package.
---"Remove apps from user profiles as well" removes the packages from all user profiles via Active Setup. This takes place on the next login.

-Features:
--NEW*: bloatware removal, reinstall and scheduling for all users via active setup
--NEW*: Provisioned package removal
--Install and uninstall selected AppX packages
--Scheduled removal (Repeated Debloating Tool)
--Security levels: Apps are categorized into security levels:
---Light: Basic bloatware and third-party apps. Safe to remove
---Heavy: Includes built-in Windows telemetry apps and non-critical tools
---Extreme: Aggressive removal. May break core Windows features
---Unfiltered: No filter on the AppX packages except for those which can damage the installation process
--The categories are contained in a whitelist. There is a hash-based compromise detection on the file. If the whitelist gets modified, it alerts on the main menu, but doesn't block any features
--The Extreme and Unfiltered modes have a password protection to avoid accidental deletion of certain packages. The password is 3141

-Known issues and limitations:
--In case of new users, bloatware removal via active setup won't work. There is a workaround by scheduling a bloatware removal for all users.

