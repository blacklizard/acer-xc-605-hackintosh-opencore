# BIOS Configuration

BIOS version: `P11.B4`

- Load Default Settings
- Advance -> Integrated Peripherals -> Legacy USB Support -> Disabled
- Authentication -> Secure Boot -> Disabled
- Boot Options -> Boot Menu -> Enabled
- Boot Options -> D2D Recovery -> Disabled


## Hidden BIOS setting
This setting can be modified using [modGRUBShell.efi](https://github.com/datasone/grub-mod-setup_var/releases/download/1.1/modGRUBShell.efi)
⚠️: These offset are only valid for the specific firmware version! Do not try to execute these commands on a different firmware! 
The modified variables will reset itself when you restore / revert to optimised defaults. 
Everytime BIOS is reset, you will need to reconfigure the hidden setting or else you will not be able to boot, you have been warned

#### Required setting
- Disable CFG Lock 

| Firmware Version | Command              |
|------------------|----------------------|
| P11.B4     |`setup_var 0x55 0x00`|


- Set DVMT pre-alloc to 64MB

| Firmware Version | Command              |
|------------------|----------------------|
| P11.B4     |`setup_var 0x2F4 0x02`|

