---------------------------
PIX32 Name Sync
v1.1
---------------------------


------------
Description:
------------

This Applescript synchronizes track names from a networked PIX recorder to a networked Behringer X32 mixer. It can be run once or on repeat. 


------
Usage:
------

To use, you will initially need to make some edits to the .plist file: 


- The X32 IP and PIX IP fields should be overwritten with the respective IP addresses of those units. 

- The Track Count field represents the amount of tracks (starting from the first one, going sequentially) you want to sync. Default is 32.

- The Directory address only needs to be changed if you place the folder anywhere other than the desktop. This value is crucial to directing the Python script to the proper folder, so it can then read the IP address from the .plist file.


Additionally, the Python script that handles OSC commands requires a library not installed on OSX by default. This library can be installed manually (search for "pyOSC") or automated using the "install_libraries" Applescript included.


****
TIP!
****
If you are using Dante Controller in conjunction with your PIX and X32, you can edit the PIX track names from the "Transmit" tab of the PIX's device view in Dante Controller. Once you click another Channel Label or otherwise leave the field it should update.


------
Fixes:
------

	v1.1
	- Improved character handling. Bad characters are defined in the script and replaced with an underscore. 
	- Added choice to repeat or run once.


-----------
Known Bugs:
-----------


--------
Credits:
--------
Open SoundControl for Python
Copyright (C) 2002 Daniel Holth, Clinton McChesney


Will Colding
Gotham Sound and Communications
willc@gothamsound.com
2/18/16