# Sublime_package_control
There are some problems when installing package control on sublime Text 3(Ubuntu 18.04), here are the solutions.

## Installing package_control
### 1 Automatic installation
Open Sublime Text 3, press Ctrl + ` to open the console. Then visit https://packagecontrol.io/installation, copy the code the paste to the console. But it may not work because of Network is not available.
### 2 Manual installation
* cd ~/.config/sublime-text-3/Packages/
* git clone https://github.com/wbond/package_control_channel.git Package\ Control 
* then select "Preferences > Browse Packages" and go back to the parent directory then go in to the "Installed Packages" directory
* download Package Control.sublime-package from https://sublime.wbond.net/Package%20Control.sublime-package and copy it to the directory in the last step
* restart sublime

### 3 Confirm that the installation was successful
select "Preferences > Package Control" then type "install" and choose "Package Control：Install Package".

## Solutions when error: There are no packages available for installation accured
select "Preferences > Browse Packages" then go to the User directory, edit the file "Package Control.sublime-settings"as follows:
```
{
    "bootstrapped": true,
    
    "channels": [
        "http://static.zybuluo.com/parkinwu/x5xsu1vjaob4hmktfexncfbz/channel_v3.json"
    ]
}
```
or download the json file to the system thenedit as follows:
```
{
    "bootstrapped": true,
    
    "channels": [
        "home/……/channel_v3.json"
    ]
}
```
the "home/……/channel_v3.json" is your absolute path

## install sublimerge 3
sublimerge 3 is a tool to find the differences between two files.
* Download Package: Sublimerge 3.sublime-package from https://www.sublimerge.com/sm3/docs/quick-start.html#installation
* select "Preferences > Browse Packages" , then copy the file downloaded to this folder.
* choose"extract here"
* restart sublime
