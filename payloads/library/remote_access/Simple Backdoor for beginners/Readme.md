# Simple Backdoor for beginners
* Author:           RonjaMaja
* Version:          1.0
* Category:         Remote access
* Target:           Microsoft Windows 10 (should work on Windows 11)
* Attackmode:       HID
* Credits to antonioCoco who wrote the powershell script
  
## Description
* opens a backdoor that you can access with Netcat
* 1 script deactivates Windows Defender
* 2 script runs the powershell script
* 3 script activates Windows Defender

## Configuration
* You just need to change 192.168.1.1 and 22
* lhost = your IP adress
* lport = the port you want to use for the Backdoor. I recommend ssh (22).
* example:
* readonly lhost="192.168.4.20"
* readonly lport="80"

## NetCat Command
    stty raw -echo; (stty size; cat) | nc -lvnp rport rhost
* rhost = IP adress from the target
* rport = the port you want to use for the Backdoor (same as lport).

## Tested on

Microsoft Windows 10 Professional Version 20H2 (PowerShell 5.1)

## requirements

The target user must belong to the 'Administrators' group.

## STATUS

| LED                 | Status                                 |
| ------------------- | -------------------------------------- |
| Yellow Single       | deactivate defender Stage              |
| Yellow Double       | Backdoor Stage                         |
| Yellow Triple       | activate defender Stage                |
| Green               | Finished                               |
