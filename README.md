[![Ezurio](/images/ezurio_logo.jpg)](https://www.ezurio.com/)

# Lyra24 Firmware

[![Lyra24-P](/images/lyra_p_and_lyra_s_render.jpg)](https://www.ezurio.com/wireless-modules/bluetooth-modules/bluetooth-5-modules/lyra-24-series-bluetooth-5-modules)
[![Silabs](/images/silabs_logo.jpg)](https://www.silabs.com)
[![Gecko SDK](/images/gecko_sdk_logo.jpg)](https://www.silabs.com/developers/gecko-software-development-kit)
[![Simplicity Studio](/images/simplicity_studio_logo.jpg)](https://www.silabs.com/developers/simplicity-studio)

This is the firmware release page for the Ezurio [Lyra24][Lyra24 series product brief] product family.

The Lyra24 product is available in the following different variants:
1. [P10 (PCB module, 10dBm output power)][Lyra24 P series datasheet],
2. [S10 (SIP module, 10dBm output power)][Lyra24 S series datasheet],
3. [P20 (PCB module, 20dBm output power)][Lyra24 P series datasheet],
4. [P20RF (PCB module, 20dBm output power with RF trace pad)][Lyra24 P series datasheet],
5. [USB Dongle (based on the PCB module with 20dBm output power)][Lyra24 P series datasheet].

---
**_Note:_** The latest available firmware releases are available on the [Lyra24 Releases Page].

Details for flashing the different image types can be found in the [Firmware options and upgrade guide] application note.

---

# Content

All firmware is offered in P10, S10, P20 and P20RF versions, depending upon the Lyra24 variant in use.

## AT Interface

The [Lyra24 AT Interface][Lyra24 AT Interface guide] application builds upon many years of AT Interface experience gained with Ezurio's BL65x range of Bluetooth modules. It offers a VSP service for cable replacement applications and GATT client and server functionality. Lyra24 is compatible with the previous Lyra series (and vice-versa) if both of them are running the latest AT Interface app. Please find [here][Lyra24 AT Interface release notes] the latest release notes.

Binaries are available for transfer using SWD and OTA and UART bootloader.

## USB

Use of the Lyra24 USB is described in the [Lyra24 USB User guide][Lyra24 USB User guide].

## Bluetooth Xpress

Bluetooth Xpress is not supported by Lyra24.
Please investigate the [Lyra][Lyra Product Landing Page] if [Bluetooth Xpress][Bluetooth Xpress] is needed.


## Bootloader

The Bootloader is required for operation of all other applications, and is also needed when performing [native C development][Native C development guide]. This should be the first application programmed to the target device.

Further details of usage of the bootloader can be found in the [Firmware options and upgrade guide][Firmware options and upgrade guide].


|   Bootloader Type  | Lyra24 P10 BOOT Pin | Lyra24 S10 BOOT Pin | Lyra24 P20 BOOT Pin | Lyra24 PRF BOOT Pin |
|--------------------|---------------------|---------------------|---------------------|---------------------|
| Ezurio |        PC07         |        PC07         |        PC07         |        PC07         |

Binaries are available for transfer using SWD only. Please note that by default all Lyra24 modules ship with the Ezurio bootloader type preprogrammed.

## DTM

Two DTM applications are available for testing the Lyra24 BLE radio performance in conjunction with the [Lyra24 P10 DVK][Lyra24 series DVK user guide], [Lyra24 P20 DVK][Lyra24 series DVK user guide], [Lyra24 P20RF DVK][Lyra24 series DVK user guide] and [Lyra24 S10 DVK][Lyra24 series DVK user guide]. These are described as follows.

Binaries are available for transfer using SWD or OTA and UART bootloader.

### BGAPI

This is used in conjunction with [tools supplied by Silabs][Silabs BGAPI DTM documentation]. Communication is performed using the [BGAPI][Silabs BGAPI description] protocol. Refer also to our [Lyra24 P BGAPI DTM][Lyra24 P BGAPI DTM Application Note] application notes for more details.

### BTSIG

This is used in conjunction with BT-SIG approved DTM test equipment. Communication is performed using the native DTM protocol as defined in the BLE specification. You can find more information in the Bluetooth SIG Bluetooth Core Specification Version 5.3 | Vol 6 (Low Energy Controller) | Part F (Direct Test Mode) which is available under [https://www.bluetooth.com/specifications/bluetooth-core-specification][Bluetooth SIG Core Specification].

[Lyra24 series product brief]: <https://www.ezurio.com/documentation/product-brief-lyra24-series>
[Lyra24 P series datasheet]: <https://www.ezurio.com/documentation/datasheet-lyra-24p>
[Lyra24 S series datasheet]: <https://www.ezurio.com/documentation/datasheet-lyra-24s>
[Lyra24 AT Interface guide]: <https://www.ezurio.com/documentation/user-guide-at-interface-application-lyra-22-24-series>
[Lyra24 USB User guide]: <https://www.ezurio.com/documentation/user-guide-lyra-24-usb>
[Lyra24 AT Interface release notes]: <https://www.ezurio.com/documentation/release-notes-lyra-24-p-s-v7-2-x>
[Lyra24 series DVK user guide]: <https://www.ezurio.com/documentation/user-guide-lyra-24p-development-kit>
[Lyra24 P BGAPI DTM Application Note]: <https://www.ezurio.com/documentation/application-note-lyra24p-bgapi-direct-test-mode>
[Lyra24 Releases Page]: <https://github.com/Ezurio/Lyra_24_Firmware/releases/tag/GA2.1>
[Silabs BGAPI DTM documentation]: <https://www.silabs.com/documents/public/application-notes/an1267-bt-rf-phy-evaluation-using-dtm-sdk-v3x.pdf>
[Silabs BGAPI description]: <https://docs.silabs.com/bluetooth/3.1/bgapi>
[Firmware options and upgrade guide]: <https://www.ezurio.com/documentation/user-guide-firmware-options-and-upgrading-lyra-series>
[Native C development guide]: <https://www.ezurio.com/documentation/user-guide-lyra-series-c-code-development>
[Bluetooth SIG Core Specification]: <https://www.bluetooth.com/specifications/bluetooth-core-specification>
[Lyra Product Landing Page]: <https://www.ezurio.com/wireless-modules/bluetooth-modules/bluetooth-5-modules/lyra-series-bluetooth-53-modules>
[Bluetooth Xpress]: <https://docs.silabs.com/gecko-os/1/bgx/latest/getting-started>
