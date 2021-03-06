rel. 1.5.2
under development
------------------------
* Added external program wait timeout

rel. 1.5.1
nov 23, 2015
------------------------
* Added output bin field (%b)
* Fixed a bug in user process creation (it was always launched as SYSTEM)
* Fixed a monitor registration/deregistration issue during setup (thanks to Thomas Schumm)
* Added temp dir field (%T)
* Fixed some bugs related to buffers' size

rel. 1.5.0
jan 24, 2013
------------------------
* Added "run as" capability; Mfilemon is now able to write to network resources

rel. 1.4.2
jul 7, 2012
------------------------
* Added compatibility with Windows 8
* Added log facility

rel. 1.4.1
jan 7, 2011
------------------------
* All fields (except %i and search fields) now can be used in command line.
* Added %r field (printer name).
* Added "Execute from" option to set working directory for user commands.

rel. 1.3.6
mar 9, 2010
------------------------
* Improved filename pattern: added some new fields, and now it's possible to specify width and alignment for each field
* Fixed bug: on UAC enabled systems (Vista, 7, 2008), if UAC was turned on the port monitor could not access the
  registry to store its information. Thus, any changes to ports were lost after machine or spooler reboot.

rel. 1.3.5
oct 25, 2009
------------------------
* Some bugfixes.

rel. 1.3.4
oct 07, 2009
------------------------
* 64-bit version released (thanks to Lars for testing).
* Should work on Windows Server 2008 and Windows 7. Anyone wants to test?

rel. 1.3.3
aug 04, 2009
------------------------
* Implemented "search fields", useful to print a multi-page document to
  many single-page files (eg. JPEG files) through Ghostscript.
  Read documentation to learn more.

rel. 1.3.2
jun 12, 2009
------------------------
* Works with Vista (thanks to Lars for testing).
* Fixed some memory leaks.
* Redirect to user defined program could fail in some circumstances.
* Improved installer.

rel. 1.3.1
may 22, 2009
------------------------
* Now you can send data to user defined command through standard input.
* Local computer / user names were used for %c / %u fields, instead of the
  computer / user names that started the print job.
* Time fields used UTC time instead of local time.
* %h field did not work properly, due to a ridiculous bug.
* I started the project using C++, and then fell back to a C coding style.
  Rewrote many lines of code in a more oop fashion.

rel. 1.3.0
may 14, 2009
------------------------
* User defined command can be executed after spooling.
* Minor enhancements and bugfixes.

rel. 1.2.0
apr 24, 2009
------------------------
* Minor enhancements and bugfixes. Added some comments to the code.
* Added support for Windows Server 2003.

rel. 1.1.0
apr 2, 2009
------------------------
* Filename pattern can now include directories that will be created recursively.
  Eg. Output path = C:\path
  Filename pattern = %u\file%i.prn
  Will create C:\path\%USERNAME% if it does not exist and then create the file inside it.

rel. 1.0.1
apr 20, 2007
------------------------
* First released version. Tested and quite stable, although not completed yet.
