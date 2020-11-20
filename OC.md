# OpenCore EFI

Download OpenCore **RELEASE** from [here](https://github.com/acidanthera/OpenCorePkg/releases/latest)


## ACPI 
- SSDT-EC.aml
- SSDT-PLUG.aml
- SSDT-HPET.aml

## Driver
- [HfsPlus.efi](https://github.com/acidanthera/OcBinaryData/raw/master/Drivers/HfsPlus.efi)
- OpenRuntime.efi - Included in OpenCore package

## Kext - Make sure to download RELEASE version
- [Lilu.kext](https://github.com/acidanthera/Lilu/releases/latest)
- [VirtualSMC.kext](https://github.com/acidanthera/VirtualSMC/releases/latest)
- [WhateverGreen.kext](https://github.com/acidanthera/WhateverGreen/releases/latest)
- [AppleALC.kext](https://github.com/acidanthera/AppleALC/releases/latest)
- [RealtekRTL8111.kext](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases/latest)
- USBPorts.kext - Use included in this repo

## Tools
- [modGRUBShell.efi](https://github.com/datasone/grub-mod-setup_var/releases/download/1.1/modGRUBShell.efi)
- OpenShell.efi - Included in OpenCore package
- CleanNvram.efi - Included in OpenCore package

## config.plist

- Use `config_igpu.plist` when having only iGPU

## EFI Folder Structure

```
EFI
├── BOOT
│   └── BOOTx64.efi
└── OC
    ├── ACPI
    │   ├── SSDT-EC.aml
    │   ├── SSDT-HPET.aml
    │   └── SSDT-PLUG.aml
    ├── Bootstrap
    │   └── Bootstrap.efi
    ├── Drivers
    │   ├── HFSPlus.efi
    │   └── OpenRuntime.efi
    ├── Kexts
    │   ├── AppleALC.kext
    │   ├── Lilu.kext
    │   ├── RealtekRTL8111.kext
    │   ├── USBPorts.kext
    │   ├── VirtualSMC.kext
    │   └── WhateverGreen.kext
    ├── OpenCore.efi
    ├── Tools
    │   ├── CleanNvram.efi
    │   ├── OpenShell.efi
    │   └── modGRUBShell.efi
    └── config.plist
```