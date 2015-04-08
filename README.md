DiskImager
==========

A Windows Disk Imager. A C#.NET utility for reading / writing SD cards and USB devices.

Licensed under GNU General Public License 3.0 or later.
Some rights reserved. See LICENSE, AUTHORS.

The current release can be downloaded [here](https://github.com/RomanBelkov/DiskImager/releases)
or [here (old link)](http://www.dynamicdevices.co.uk/downloads/DiskImager.Installer.msi)

Utility was tested on Windows 7 and Windows 8/8.1/8.1 Pro.

(Please feed back any platform testing you do, or any issues you encounter. Thanks.)

## Description ##
This utility is a .NET implementation of Win32DiskImager with a couple of features authors wanted to use:

- writing images to a number of SD cards at once

- reads/writes images to/from compressed file formats: ZIP, TGZ, GZ, XZ

- remembers the last file you read/wrote 

- unmounts drives after write

- provides more file filters within file dialog for typical image files (.img, .bin, .sdcard)

- it also *might* be slightly faster when dealing with uncompressed read/write

*NOTE: This application is under development and could possibly cause damage to your computer drive(s). We cannot take responsibility for any damage caused or losses incurred through use of this utility. Use at own risk!*

Credits: Inspired by the excellent Win32DiskImager.

## ChangeLog ##

1.4.0 08/04/2015 RB Simplified UI

1.3.2 25/03/2015 RB Added post-action notification & resolved issue when MBR's with more than one partition were read incorrectly

1.3.1 16/03/2015 RB Added MultiThreaded XZ compression & helping tooltips

1.3.0 19/02/2015 RB Added XZ support

1.2.2 21/01/2015 RB Added 'Remove drives after write' and drew new GUI

1.2.1 14/01/2015 RB Added Russian localization and tweaked GUI a bit.

1.2.0 06/01/2015 RB Added ability to write the same image to many SD simultaneously. Changed the look of GUI. 
	

1.1.0	12/05/14	AJL		Updated to use latest SharpZipLib as we were encountering (de-)compression errors with the previous version.
							Added the option to truncate the read image based on the partition sizes found in the master boot record on the disk/stick.
							Improved logging of sizes read and written.

1.0.3	30/04/14	AJL		Added warning dialog box when there's a write error.

1.0.2	09/11/13	AJL		Added support for reading and writing directly to compressed formats: .zip, .tgz, .gz

	Testing - Windows 8.1 Professional

1.0.1	08/11/13	AJL		Refactoring for cleanup. Fixed issue with SEH exception due to SafeHandle disposal.

	Testing - Windows 8.1 Professional

1.0.0	08/11/13	AJL		Initial Commit. Reads and Writes SD cards.

	Testing - Windows 8.1 Professional

Contact
=======
Roman Belkov  - romanbelkov@gmail.com

Alex J Lennon - ajlennon@dynamicdevices.co.uk
