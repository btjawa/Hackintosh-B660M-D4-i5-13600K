# Hackintosh-B660M-D4-i5-13600K

| OpenCore | macOS Version |
| -------- | ------------- |
| **OpenCore 1.0.6** | **macOS 15 Sequoia** |

## Notes

Since [itlwm](https://github.com/OpenIntelWireless/itlwm) is currently stuck at v2.3.0 (corresponded to macOS 14 Sonoma), native Wi-Fi and Bluetooth are not **yet** supported on macOS 15 Sequoia.

There are some workarounds, but the best solution is always waiting for updates to itlwm.

**1. [OCPL-Mod](https://github.com/laobamac/OCLP-Mod)**

**2. Device Spoofing (manual)**

Although the Bluetooth was unstable in practice, it was at least usable.

You could refer to the tutorial below:

- [Native-Wifi-for-Hackintoshes-with-Intel-Wireless-cards-on-macOS-sequoia](https://github.com/randomappleboi/Native-Wifi-for-Hackintoshes-with-Intel-Wireless-cards-on-macOS-sequoia)

**3. Software simulation**

Use `itlwm.kext` with `HeliPort.app` instead of `AirportItlwm.kext`. Bluetooth will not be available.

---

The included USB Mapping was customized based on my PC, you may need to [customize](https://github.com/USBToolBox/tool) yours to match your setup.

The SMBIOS data was already desensitized, please generate it yourself by using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS).

## Specification

| Specifications | Detail |
| -------------- | ------ |
| Motherboard    | ASUS TUF GAMING B660M-PLUS WIFI D4 |
| Processor      | Intel Core i5-13600K |
| Memory         | Corsair Vengeance DDR4 16GB × 2 @3200MHz |
| Storage        | WD_BLACK SN770 2TB + WD Blue SN580 2TB |
| Integrated Graphics | Intel UHD Graphics 770 |
| Dedicated Graphics | Radeon RX 5500 XT |
| Integrated Audio | Realtek ALC897 |
| Wireless       | Intel Wi-Fi 6 AX201 |
| Ethernet       | Realtek RTL8125 (2.5GbE) |

## Credits

- [acidanthera/OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)
- [corpnewt/ProperTree](https://github.com/corpnewt/ProperTree)
- [corpnewt/GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)

I _refactored_ the whole OpenCore config this time! Thanks for the amazing tutorial written by [Dortania](https://github.com/dortania) team!

- [dortania/OpenCore-Install-Guide](https://github.com/dortania/OpenCore-Install-Guide)