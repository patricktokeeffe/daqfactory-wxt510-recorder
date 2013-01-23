WXT510 in DAQFactory v1 README
Nov 2, 2010 | patrick.t.okeeffe@gmail.com

This machine is fully backed up and can be used for collecting WXT data at the dairy. However, this version of the DAQFactory program is quite lacking in a few areas still:
	- No recognition or logging of rain or hail events
	- Logs wind direction unadjusted for azimuth or declination
	- Won't maintain changes to directories if restarted
	- Can't recognize when WXT is off/not connected
	- Averaged datasets aren't aligned to nice intervals 
	- Diagnostic file will have mismatched records
	- Display is Visually confusing
	- File-splitting by length (daily, hourly, etc) untested

Further, there are two .bat files for startup & shutdown. Launching the forcedCleanStartup.bat will kill leftover DAQFactory.exe processes prior to starting DAQFactory (NECESSARY! since DF won't release COM ports otherwise); the forcedCleanShutdown.bat is called automatically upon exiting.