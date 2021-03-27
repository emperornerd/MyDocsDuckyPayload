This is intended for the standard ducky firmware. It's designed to copy to a file share you've already setup. You'll need to update a handful of values before you compile this. 
You can use the compiler created by the Ducky's creator (Darren), here: https://github.com/hak5darren/USB-Rubber-Ducky
Or you may use this very simple online tool: 
https://ducktoolkit.com/encode

By default this copies only spreadsheets. But you can copy *.* (everything) instead of *.xlsx. Or you can choose to do *.pdf, etc. 

The laptop I wrote this on is called "i7laptop" and I created a share called, "payloadshare". You will need to input the destination and hostname replacing my own. 

Note that the CAPS key light will toggle (on if it was off and off if it was on) when the script is done. 

XCOPY Flags (feel free to change them): 
https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/xcopy 

/Y /C /Q /R /K

/y: supresses prompting for overwrite
/C: ignore errors
/S: Copies sub-directories
/E: Copies ALL sub-directories 
/Q: Suppress display of XCOPY messages
/R: Copies read only files
/K: Retain read-only attribute
