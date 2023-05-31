### Changelog
2.26.1
* Scroll bar now enabled in full-screen mode
* Added a search button in the connections window
* Fixed some focus issues

2.26.0
* Configuration: Backup to and restore from file
* Cluster Mode: New option to adjust Multi-Input selection for a whole row/column
* Configuration: New option "Tab Prefix" for each folder
* Connection Groups: New option to prevent closing all connections

2.25.2
* Bug fix: "Reconnect gracefully" terminates the PuTTY window when using Jump Server mode "SSH Proxy" and the proxy host is not reachable
* Bug fix: Fixed architecture detection for Windows under Help->Info
* Bug fix: Variables did not get properly replaced when using WSL Starter
* MSI installer: Changed default install scope to "user" (see point 30 in the FAQ section)

2.25.1
* Bug fix: "Reconnect gracefully" doesn't work when using Jump Server mode "SSH Proxy"

2.25.0
* Native arm64 build for Windows on Arm now available
* Dropped support for x86 (32-bit)
* Improved implementation makes the Dll "lib/WinSSHTerm.dll" now obsolete
* Configuration Window: Tab key now moves to the next property
* Build environment: Upgrade to Visual Studio 2022

2.24.0
* New option to append custom command line parameters for Pageant, useful e.g. when using PuTTY CAC (File->Prefernces->Pageant)
* Bug fix: Ignored private key file when using Jump Server mode "SSH Proxy" (thanks to drizzt09)
* Bug fix: Possible race condition in Script Runner

2.23.3
* Bug fix: Focus issues when "Multi-Input" was not enabled (thanks to mxmihai)

2.23.2
* Bug fix: Setting the password command line option for PuTTY/Plink/WinSCP even if password is empty
* Bug fix: Minor focus issues

2.23.1
* SECURITY FIX: In version 2.23.0, temporary files are used for PuTTY's new command line option "-pwfile". In some cases these temporary files did not get deleted, that means files containing the password might be inside your temporary folder. So be sure to delete your temporary files folder (probably "C:\Users\<USER>\AppData\Local\Temp\") if you use passwords to authenticate for your ssh sessions. Instead of using temporary files, now in version 2.23.1 shared memory is used. All password files will be deleted after they got read by PuTTY/Plink. Additionally, only when PuTTY will read the password file, the password is actually written. If you don't use passwords for ssh authentication, you are not affected by this issue.
* Bug Fix: WinSSHTerm not exiting properly in some cases when the features "Script Runner" or "Check Access" was used

2.23.0
* PuTTY: Replaced command line option "-pw" with the new and more secure option "-pwfile", so if passwords are used for authentication, it is required to use PuTTY/Plink 0.77 or higher
* Improvement: WinSSHTerm could freeze in some cases
* Bug fix: In some cases it was not possible to delete the file "lib\WinSSHTerm.dll"
* Bug fix: When selecting "Display context menu" as copy&paste behaviour for the terminal, right clicking in a terminal window the first time would close the context menu 

2.22.0
* Jump Server: Implemented the new PuTTY feature "SSH Proxy" (>= 0.77)
* WSL Starter: Several bug fixes, WSL variables can now be used in the connection configuration
* Info dialog: Version check added
* Color Scheme: Improvements to the default color scheme "WinSSHTerm light"
* Multi-Input Scripts: Bug fix: Remember current script text when closing
* Copy Files: Bug fix: Pop-up when Plink is not installed
* Rename Tab: Bug fix when moving tab to another window
* Quick connect: Bug fix: Replace variables in tab title
* Removed support for KiTTY
* Added URL to the support forum (Help->Support)

2.21.0
* New feature: Toggle Full Screen for the current session with ALTGR+ENTER
* Bug Fix: Alt-Tab: Needs to press tab twice
* Bug Fix: Detaching the terminal when using multiple monitors always detaches on the primary monitor
* Search, History, QuickConnect: These windows won't get closed when WinSSHTerm looses focus
* Tab context menu: Compacted PuTTY menu items into a sub menu / New menu item "Toggle Full Screen"
* WSL Starter: Autostart SSH server will now be triggered on demand, when opening a WSL connection
* WSL Starter: For a WSL connection, it is now sufficient to set the host and port
* Color Scheme: Default color scheme now "WinSSHTerm light" / Adjusted color scheme "WinSSHTerm light"
* Color Scheme: New button to set the default light tab color (used in "WinSSHTerm light")
* Color Scheme: Default background color now equal to "Tab Color" if "Custom Tab layout" is enabled
* new unsupported warning if an architecture mismatch was detected (Popup, Title Bar)
* new built-in variable CON.PASSWD to access the SSH password (see point 26 in the FAQ section)

2.20.1
* Bug fix: Quick Connect: Open connection with "Enter" key
* Bug fix: Connection Filter: Search for Pattern Groups now functional
* Bug fix: Connection Filter: Tab order improved

2.20.0
* New feature "Connection Filter": Filter connections quickly with include and/or exclude patterns (Navigate->Connection Filter)
* Script Runner/Cluster Mode: New button "Con filter" to quickly access the new feature "Connection Filter"
* Script Runner/Cluster Mode: CTRL+A selects all connections
* Cluster Mode: New option to add a connection or all connections inside a folder from the Connections window (Right Click->Add to Cluster Mode)
* Cluster Mode: Remember the column count, default is 2
* Holding "SHIFT" and opening a connection will open the connection in the next window
* PuTTY option "Change Settings..." now available in the tab context menu, which lets you change settings like font size while the session remains active
* Disabled editing the connection name by clicking on it (still possible with F2 or "Right click"->Rename)
* Info Dialog: New section for Windows, added UBR to the build number for Windows
* Bug fix: Focus issue when clicking on the title bar and then on a menu item

2.19.1
* Bug fix: Fixed some focus issues
* Script Runner: Output CustomId if not empty

2.19.0
* new feature "WSL Starter": Easy access to WSL on Windows (Tools->WSL Starter)
* Bug fix: Now correctly restoring the window in some cases with multiple monitors

2.18.0
* Multi-Input Scripts: Added possibility to search scripts

2.17.0
* Copy Files: New option to use WinSCP's native tunneling feature (File->Preferences->Copy Files->Global Settings)
* Copy Files: By default, WinSCP's option to "Optimize connection buffer size" is now disabled
* Connection groups are now listed in the "Cons" menu

2.16.0
* Re-attaching the terminal window now possible (new Option under File->Preferences->General)
* Cluster Mode: new option to set another SSH user (Cluster Mode->Open as user)
* Search Window: Adjusting width of drop down box to fully display the search results
* Feature 'Convert OpenSSH Key': improved implementation
* KiTTY: after resizing the terminal font with CTRL+Mousewheel the terminal window size now gets correctly adjusted
* Minor changes to the GUI
* Build environment: Upgrade to Visual Studio 2019

2.15.0
* Check Access: Interactions now possible (like storing a new host key into cache with "y")
* Check Access: Additionally checking access for the jump server if configured
* Check Access: In case a password is used for a jump server, the password is now hidden from check access output
* Improved implementation for setting the terminal font size
* New shortcut "ALTGR+J" for "Send to quick-connect" feature
* Minor changes to the GUI
