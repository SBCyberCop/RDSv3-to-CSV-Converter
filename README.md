# RDSv3 .DB to .CSV Converter
Convert RDSv3 DB Files to CSV for import.

[Current RDS Hash Sets from NIST.gov](https://www.nist.gov/itl/ssd/software-quality-group/national-software-reference-library-nsrl/nsrl-download/current-rds)

# Instructions
* Download zip [[Download]](https://github.com/SBCyberCop/RDSv3-to-CSV-Converter/archive/refs/heads/main.zip)
* Extract EXE (and config if needed)
* Place EXE (and config) into the same folder as the RDS .DB file and signatures file.
* Run the EXE

**Be patient ... The Modern PC	and Legacy PC .DB are around 113 GB ... It make take several hours to  convert these files to .csv**

# Requirements
* sqlite3.exe [[Download]](https://www.sqlitetutorial.net/download-install-sqlite/)
* sed.exe [[Download]](https://sourceforge.net/projects/gnuwin32/files//sed/4.2.1/sed-4.2.1-setup.exe/download)

# Compatibility
* (+) Minimal
* (+) Full
* (+) Windows 10
 * (?) Windows 11 or < Windows 10
* (+) PowerShell Version 5.1.19041.2673

# Config.ini (optional)
```ini
[General]
#BypassPTC=1
;Remove the # to enable Bypass Prompt To Continues and Run the script autonomously unless error'd.
#SkipHashCheck=1
;Remove the # if the program should not check the DB hash with the signature file.
#SkipAdminCheck=1
;Remove the # if the program should not check if the program is running in admin mode.
#NumOfChunks=4
;Remove the # and change the value to either 4, 6, 8, 12.  Higher numbers for larger DB files
;or if memory problems are occuring.
#BeepOn=0
;Remove the # if the program should not give an audio beep during events.
#ExitOnEnd=1
;Remove the # if the program should close automatically after successful conversion.
#ShowInFolder=1
;Remove the # if you want an explorer window to appear showing where the newly created file is.
```
