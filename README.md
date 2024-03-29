# RangemanSync
This is a custom built Casio GPR-B1000 sync application that has GPX export and OpenStreetMap based maps. I don't have any documentation about the communication protocol of the watch so I had to figure out everything by myself. This is the reason why you can expect some minor differences between my sync app and G-Shock Connected.

## About myself
I'm a .NET backend one-man developer so please don't expect 1 minute fixes, or instant replies from me. I'm only doing this project in my freetime, but I'll try to do my best to answer questions / address potential issues.

## Android OS version requirement
The app has been tested on Android 12 and 13 versions.
Unfortunately it turned out the minimum OS version number of the apk package is set to a lower number so the app can be started on Android 7 as well, but the app won't work on Android 7 due to problems with getting the right permissions.

## Installation
Use Google Play store to install it.

(demo) [https://play.google.com/store/apps/details?id=com.Szilamer.RangemanSyncDemo]

(full version) [https://play.google.com/store/apps/details?id=com.Szilamer.RangemanSync]

Please "force stop" or uninstall the G-Shock Connected application before trying to use this sync app. 
These are created for using the same bluetooth connection to the same watch, so this step is needed to avoid the conflicting usage.

The following permissions are needed by the app:
Location
Nearby devices discovery (bluetooth)

## Limitations of the unlicensed version
Only the download headers button can be used on the download tab to test the communication between your watch and the phone.

## Using the download tab
Every route on the watch consists of two parts:
- Route header
- Multiple GPS coordinates under the selected route header

**To start downloading route headers the first step is pressing the Download headers button on the Download tab:**

![1](https://user-images.githubusercontent.com/111239271/205501396-a3754867-a9e6-4f3c-b7c2-c621c1db4bac.jpg)

**The app is switched to connection mode, so the following page will be displayed for you:**

![2](https://user-images.githubusercontent.com/111239271/205501484-06cb3a3c-509f-4b2c-bdb2-475c3a32bb11.jpg)

**It's time to connect the watch now, so please press and hold the bottom left button:**

![7](https://user-images.githubusercontent.com/111239271/205501648-ebd2b014-b79f-408f-a8f3-ad22fa5a9d74.jpg)

**Please wait a little bit and the route records downloaded from the watch will be shown to you:**

![3](https://user-images.githubusercontent.com/111239271/205501779-2f2fb613-521c-482a-8db3-c4d84b821b0f.jpg)

**Select one header record from the list by clicking on it:**

![4](https://user-images.githubusercontent.com/111239271/205501872-8be25ca2-07c3-47e8-8818-b5b31f884882.jpg)

**Then you can press the "Save as GPX" button to start downloading the GPS coordinates as a GPX format**

**You can use the save as dialog as soon as the GPX file is ready:**

![5](https://user-images.githubusercontent.com/111239271/205501976-f6242884-a075-4c08-a630-1e4d7fa8a70c.jpg)

## Using the maps tab

The purpose of this tab is to send GPS coordinates to the watch.
These coordinates can be created by clicking on the map to place 'nodes'.
Every node has a label and the watch can handle these type of nodes:

- Start, this is marked as 'S' on the map
- Goal, this is marked as 'G' on the map
- Interim route points: these are marked with 1..9 on the map

![map1](https://user-images.githubusercontent.com/111239271/205502643-e7c193ed-3d98-4371-baf9-0cb017d9741e.jpg)

## Support / help

Please use the error reporting feature of config tab if you experience any weird error messages during running the application.
Just select 'Send log files to support email' and press apply changes.
A new email message will be automatically created with the support email address, log files in the attachment.
**Please be aware that log files can contain sensitive information about you, GPS coordinates.**
So please don't send the log files to me if you'd like to keep this information private.

## Known issues

The sending and receiving is stable based on my tests. Pressing the disconnect button during in the middle of sending coordinates (maps tab) very rarely caused one unusal side effect on my watch : The time, date and the time zone was reset to the factory default 2015, Tokyo settings. The solution is easy if you ever encounter this issue : just set it back to the current time and date by using the adjust button, or use the receiving button (bottom right) to select the GPS based time synchronization: time (gps)

