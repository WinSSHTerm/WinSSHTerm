### Changelog
2.19.1
* Bug fix: Fixed some focus issues

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
