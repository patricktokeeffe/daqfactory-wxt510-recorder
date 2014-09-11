WXT510 in DAQFactory
====================

> This project is no longer actively developed. The last known update occurred 
> 2010-Nov-2. Users are encouraged to use an SDI-12 compatible datalogger such 
> as the CR1000 or CR3000 by Campbell Scientific Inc.

### Some notes

Use `forcedCleanStartup.bat` to start things; it will kill any zombie 
DAQFactory.exe processes prior to starting DAQFactory, which ensures COM ports
are released. `forcedCleanShutdown.bat` is called automatically upon exiting
DAQFactory.

The low-level driver for WXT510 is maintained in 
[a separate Git repository](https://github.com/patricktokeeffe/daqfactory-pVaisala-WXT510.git).

### Future work

- No recognition or logging of rain or hail events
- Logs wind direction unadjusted for azimuth or declination
- Won't maintain changes to directories if restarted
- Can't recognize when WXT is off/not connected
- Averaged datasets aren't aligned to nice intervals 
- Diagnostic file will have mismatched records
- Display is Visually confusing
- File-splitting by length (daily, hourly, etc) untested

### License

This work is licensed under [The MIT License](http://opensource.org/licenses/mit-license.html).

### Disclaimer

This work is not affiliated with or endorsed by Vaisala, Inc., the maker of
the WXT510 weather transmitter.
