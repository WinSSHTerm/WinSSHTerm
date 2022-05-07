### Changelog
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
