# AMD Ryzen Hackintosh - Opencore EFI for Asrock B450 series


## Specification
| **Component** | **Model** |
| ------------- | --------- |
| CPU | AMD Ryzen 5 3600 @ 3.6GHz |
| Motherboard | Asrock B450 Series |
| RAM | 32GB (2 x 16GB) Corsair Vengeance RGB @ 3200 CL16 |
| Audio Chipset | ALC892/897 |
| GPU | Gigabyte RX 580  |
| Ethernet | RTL8111 1GbE |
| OS Disk (Nvme/Sata3) | Samsung 970 EVO+ 500GB | Samsung 860 EVO 250GB |

**macOS version**: Mojave 11.2 (Can be use for 10.15.x also)  

**OpenCore version**: 0.5.6

**SMBIOS**:  iMacPro1,1

## How to use
  1. Create directory "EFI" in your EFI partition (e.g. pendrive or hard drive)
  2. Clone this repo and paste directiories "BOOT" and "OC" onto created directory
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as model select **iMacPro1,1**.
  4. Open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic. Set MLB (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values.
  5. Boot it!  

## Disclaimer

This documentation is published for the sole purpose of learning and tech enthusiasm and with no guarantees of any kind, I’m not responsible of any harm of any kind or loss of data that may occur.
