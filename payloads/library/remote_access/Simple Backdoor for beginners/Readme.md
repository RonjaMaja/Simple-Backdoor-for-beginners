# Title:      
 Simple Backdoor for beginners
## Description
* 1) script deactivates Windows Defender
* 2) script runs the powershell script
* 3) script activates Windows Defender
* Author:           RonjaMaja
* Version:          1.0
* Category:         Remote access
* Target:           Microsoft Windows 10 (should work on Windows 11)
* Attackmode:       HID
* Credits to antonioCoco who wrote the powershell script

## Configuration
You just need to change lhost and lport
lhost = your IP adress
lport = the port you want to use for the Backdoor. I recommend ssh (22).

## NetCat Command
     stty raw -echo; (stty size; cat) | nc -lvnp rport rhost
rhost = the target
rport = the port you want to use for the Backdoor (same as lport).

# TESTED ON
===============
Microsoft Windows 10 Professional Version 20H2 (PowerShell 5.1)

# REQUIREMENTS
===============
The target user must belong to the 'Administrators' group.

# STATUS
===============
Magenta solid ................................... SETUP
Yellow single blink ............................. STAGE1
Yellow double blink ............................. STAGE2
Yellow triple blink ............................. STAGE3
