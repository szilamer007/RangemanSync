# RangemanSync
This is a custom built Casio GPR-B1000 sync application that has GPX export and OpenStreetMap based maps

## Installation
Just use the latest APK file on the releases page. 
The complete install process and steps are in this Youtube video : 

[Installation video](https://youtu.be/E3N8D17JhdE)

Please "force stop" or uninstall the G-Shock Connected application before trying to use this sync app. 
These are created for using the same bluetooth connection to the same watch, so this step is needed to avoid the conflicting usage.

The following permissions are needed by the app:
Location
Nearby devices discovery (bluetooth)

## Licensing & license fee
This application is not completely free, but the current license fee is very low , so that's 13 EUR for 2 years.
This is completely handled by an external licensing provider called netlicensing.io. 
I'm only asking this small donation to support my coffee consumption during the development and keep me motivated.
This app was originally created for myself to make my life easier during hiking, and I think the current version completely satisfies my needs, but I can continue it if I see enough interest.

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




