---
title: "Project My Screen not working"
date: ""
categories: 
  - "blogs"
tags: 
  - "screen-application"
  - "windows-phone"
coverImage: "2014-04-23_11h56_23.png"
---

While trying out Project My Screen for Windows Phone 8.1, I had the problem that it only showed a black screen and did not ask my phone to connect. This is due to old drivers. Other sites told me to remove the drivers and just replug it. The solution, however, requires a couple of steps more.

 

When you have the issue, try these steps:

1. Uninstall the Project My Screen application
2. Go to Device Manager in your Control Panel of Windows
3. Under Portable Devices, right click your phone and click Uninstall.
4. Under Universal Serial Bus Devices, you should have 3 "WinUsb Device"'s. Right click them one at a time and check the "Delete the driver software for this device" checkbox if possible.
5. Unplug your Windows Phone 8.1 device
6. Reinstall the Project My Screen application
7. After the installation plug your phone in again and start the Project My Screen application. You should now receive a popup to allow screen projection.
