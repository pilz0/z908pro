# z908pro

## What do we know about the Wifi Cam Chip

It is probably a Bouffalo Lab Chip.

The boot log contains a reference to the BLSP_Boot2, which is a bootloader for Bouffalo Lab Chips. We grepped the binary for some strings from the boot log and found some matches, so we are quite sure that the chip is a Bouffalo Lab Chip. Not sure which one though.

After the bootloader log it switches to random binary garbage which is probably output of the firmware. Maybe it just changes the baudrate or something like that.
## The rest of Chips
### Motorcontrollers
For the motor of the Cam there is a Mixic MX116H motorcontroller
## Battery
The Battery is a 2000 mah 3,7 Volt LiPo.
The Chip on the Battery Controller says "LC 9" and has some resistors and Capasitors around it. It is connected to the USB Port.
## About the Drone
Aliexpress Link: https://de.aliexpress.com/w/wholesale-z908pro.html
## Bootloader Log

```
system clock=000000A0BLSP_Boot2_CP:Dec 22 2021,19:38:18
commit id=9f75399d1831379c92c2b0d58faee73a3af03277
xActive PT:0,0ig
MFG not foundGet FW ID:0
Name=FW_CPU0
Age=0
active Index=0
active Address=00060000
Check Img
Get FW ID:1
Entry not found
Boot start
Media boot main
R header from 00060000
sign 0,encrypt:1
R IV
Cal hash
Success
0,0
Success
CPU 1 not boot
Found One img Only
49b7da91,19879f81
49b7da91,19879f81
00061000,00000000
00061000,0000000f
CPU Count 2,0
Counter value=15810757
     +++++ RANDOM BINARY GARBAGE +++++
```
