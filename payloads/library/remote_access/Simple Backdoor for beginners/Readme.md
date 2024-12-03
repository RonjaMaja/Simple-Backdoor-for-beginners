# Title:      
 			  Simple Backdoor for beginners
## Description:      
  			  1) script deactivates Windows Defender
  			  2) script runs the powershell script
  			  3) script activates Windows Defender
# Author:           RonjaMaja
# Version:          1.0
# Category:         Remote access
# Target:           Microsoft Windows 10 (should work on Windows 11)
# Attackmode:       HID
# Credits to antonioCoco who wrote the powershell script
#
# TESTED ON
# ===============
# Microsoft Windows 10 Professional Version 20H2 (PowerShell 5.1)
#
# REQUIREMENTS
# ===============
# The target user must belong to the 'Administrators' group.
#
# STATUS
# ===============
# Magenta solid ................................... SETUP
# Yellow single blink ............................. STAGE1
# Yellow double blink ............................. STAGE2
# Yellow triple blink ............................. STAGE3

# Faster SMB Exfiltrator V 2.0

* Author: Hak5Darren
* Props: ImNatho, mike111b, madbuda, jblk01
* Version: Version 1.6.1
* Target: Windows XP SP3+ (Powershell)
* Category: Exfiltration
* Attackmodes: HID, Ethernet
 
## Description

Exfiltrates select files from users's documents folder via SMB.
Liberated documents will reside in Bash Bunny loot directory under loot/smb_exfiltrator/HOSTNAME/DATE_TIME
