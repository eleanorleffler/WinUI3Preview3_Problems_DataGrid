# WinUI3Preview3_Problems_DataGrid

This repository contains two solutions with sample code demonstrating the DataGrid in both UWP and WinUI3 Desktop.

The UWP sample code works as expected. However, the WinUI3 Desktop sample code crashes when the DataGrid is resized to have a scrollbar or has enough data to require the window to have a scrollbar.

----

**Describe the bug**

The CommunityToolKit DataGrid displays and is scrollable in UWP In WinUI3 Preview3 Desktop, the DataGrid does display but crashes when scrollbar is needed. See Screenshot#1 for current behavior.

**Steps to reproduce the bug**

1. Clone [WinUI3Preview3 Problems DataGrid repository](https://github.com/eleanorleffler/WinUI3Preview3_Problems_DataGrid).
2. Go to the DataGridWinUIPreview3 folder.
3. Open the DataGridWinUIPreview3 solution in Visual Studio 2019 Preview.
3. Build and run with Debug x64.
4. If the window is big enough to display all 10 rows, adjust the screen to introduce the scrollbar vertically or horizontally.

**Expected behavior**

We expect the DataGrid to be scrollable when window is unable to display all of the data in the DataGrid - the same behavior we saw in UWP. See Screenshot#2

**Screenshots**

Screenshot#1 - Current Behavior

Screenshot#2 - Expected Behavior

**Version Info**

NuGet package version: 

[Microsoft.VCRTForwarders.140 1.0.6]
[Microsoft.WinUI 3.0.0-preview3.201113.0]

Targeting:
Target: Universal Windows
Target version: Windows 10, version 1809 (10.0; Build 17763)
Min version: Windows 10, version 1803 (10.0; Build 17134)

Windows app type:
| UWP              | Win32            |
| :--------------- | :--------------- |
| 		Yes 	   |  				  |

| Windows 10 version                  | Saw the problem? |
| :--------------------------------- | :-------------------- |
| Insider Build (xxxxx)              | 						 |
| May 2020 Update (19041)            | 						 |
| November 2019 Update (18363)       | 						 |
| May 2019 Update (18362)            | 						 |
| October 2018 Update (17763)        | 			Yes			 |
| April 2018 Update (17134)          | 						 |
| Fall Creators Update (16299)       | 						 |
| Creators Update (15063)            | 						 |

| Device form factor | Saw the problem? |
| :----------------- | :--------------- |
| Desktop            | 		Yes			|
| Xbox               | 					|
| Surface Hub        | 					|
| IoT                | 					|

**Additional context**
