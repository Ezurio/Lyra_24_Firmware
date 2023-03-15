[![Laird Connectivity](/images/laird_connectivity_logo.jpg)](https://www.lairdconnect.com/)

# Lyra24 Firmware

[![Lyra24-P](/images/lyra_p_and_lyra_s_render.jpg)](https://www.lairdconnect.com/wireless-modules/bluetooth-modules/bluetooth-5-modules/lyra-series-bluetooth-53-modules)
[![Silabs](/images/silabs_logo.jpg)](https://www.silabs.com)
[![Gecko SDK](/images/gecko_sdk_logo.jpg)](https://www.silabs.com/developers/gecko-software-development-kit)
[![Simplicity Studio](/images/simplicity_studio_logo.jpg)](https://www.silabs.com/developers/simplicity-studio)

This is the firmware release page for the Laird Connectivity [Lyra24][Lyra24 product brief] product family.

The product is available in [P10 (PCB module)][Lyra24 P10 module datasheet], [P20 (PCB module)][Lyra24 P10 module datasheet] and [PRF (PCB module)][Lyra24 PRF module datasheet] variants

---
**_Note:_** The latest available firmware releases are available on the [Lyra24 Releases Page].

Details for flashing the different image types can be found in the [Firmware options and upgrade guide] application note.

---

# Content

All firmware is offered in P10, P20 and PRF versions, depending upon the Lyra24 variant in use.

## AT Interface

The [Lyra24 AT Interface][Lyra24 AT Interface guide] application builds upon many years of AT Interface experience gained with Laird Connectivity's BL65x range of Bluetooth modules. It offers a VSP service for cable replacement applications and GATT client and server functionality. Please find [here][Lyra24 AT Interface release notes] the latest release notes.

Binaries are available for transfer using SWD and OTA and UART bootloader.

## Bluetooth Xpress

Bluetooth Xpress is not supported by Lyra24. 
Please investigate the [Lyra][Lyra Product Landing Page] if [Bluetooth Xpress][Bluetooth Xpress] is needed.


## Bootloader

The Bootloader is required for operation of all other applications, and is also needed when performing [native C development][Native C development guide]. This should be the first application programmed to the target device.

Further details of usage of the bootloader can be found in the [Firmware options and upgrade guide][Firmware options and upgrade guide].


|   Bootloader Type  | Lyra24 P10 BOOT Pin | Lyra24 P20 BOOT Pin | Lyra24 PRF BOOT Pin |
|--------------------|---------------------|---------------------|---------------------|
| Laird Connectivity |        PC07         |        PC07         |        PC07         |

Binaries are available for transfer using SWD only. Please note that by default all Lyra24 modules ship with the Laird Connectivity bootloader type preprogrammed.

## DTM

Two DTM applications are available for testing the Lyra24 BLE radio performance in conjunction with the [Lyra24 P10 DVK][Lyra24 P10 DVK user guide], [Lyra24 P20 DVK][Lyra24 P20 DVK user guide]
and [Lyra24 PRF DVK][Lyra24 PRF DVK user guide]. These are described as follows.

Binaries are available for transfer using SWD or OTA and UART bootloader.

### BGAPI

This is used in conjunction with [tools supplied by Silabs][Silabs BGAPI DTM documentation]. Communication is performed using the [BGAPI][Silabs BGAPI description] protocol. Refer also to our [Lyra24 P BGAPI DTM][Lyra24 P BGAPI DTM Application Note] application notes for more details.

### BTSIG

This is used in conjunction with BT-SIG approved DTM test equipment. Communication is performed using the native DTM protocol as defined in the BLE specification. You can find more information in the Bluetooth SIG Bluetooth Core Specification Version 5.3 | Vol 6 (Low Energy Controller) | Part F (Direct Test Mode) which is available under [https://www.bluetooth.com/specifications/bluetooth-core-specification][Bluetooth SIG Core Specification].

[Lyra24 product brief]: <https://www.lairdconnect.com/documentation/product-brief-lyra-series>
[Lyra24 P10 module datasheet]: <https://www.lairdconnect.com/documentation/datasheet-lyra-p>
[Lyra24 P20 module datasheet]: <https://www.lairdconnect.com/documentation/datasheet-lyra-p>
[Lyra24 PRF module datasheet]: <https://www.lairdconnect.com/documentation/datasheet-lyra-s>
[Lyra24 AT Interface guide]: <https://www.lairdconnect.com/documentation/user-guide-interface-application-lyra-series>
[Lyra24 AT Interface release notes]: <https://www.lairdconnect.com/documentation/release-notes-lyra-series-x31171>
[Lyra24 P10 DVK user guide]: <https://www.lairdconnect.com/documentation/user-guide-lyra-p-development-kit>
[Lyra24 P20 DVK user guide]: <https://www.lairdconnect.com/documentation/user-guide-lyra-p-development-kit>
[Lyra24 PRF DVK user guide]: <https://www.lairdconnect.com/documentation/user-guide-lyra-p-development-kit>
[Lyra24 P BGAPI DTM Application Note]: <https://www.lairdconnect.com/documentation/application-note-using-bgapi-direct-test-mode-lyra-p>
[Lyra24 Releases Page]: <https://github.com/LairdCP/Lyra_Firmware/releases/tag/GA1.1>

[Silabs BGAPI DTM documentation]: <https://www.silabs.com/documents/public/application-notes/an1267-bt-rf-phy-evaluation-using-dtm-sdk-v3x.pdf>
[Silabs BGAPI description]: <https://docs.silabs.com/bluetooth/3.1/bgapi>

[Firmware options and upgrade guide]: <PickleRick2002https://www.lairdconnect.com/documentation/user-guide-firmware-options-and-upgrading-lyra-series>
[Native C development guide]: <https://www.lairdconnect.com/documentation/user-guide-lyra-series-c-code-development>
[Bluetooth SIG Core Specification]: <https://www.bluetooth.com/specifications/bluetooth-core-specification>

[Lyra Product Landing Page]: https://www.lairdconnect.com/wireless-modules/bluetooth-modules/bluetooth-5-modules/lyra-series-bluetooth-53-modules
[Lyra product brief]: <https://www.lairdconnect.com/documentation/product-brief-lyra-series>
[Bluetooth Xpress migration guide]: <https://www.lairdconnect.com/documentation/user-guide-bluetooth-xpress-bgx-migration-lyra-modules>
[Bluetooth Xpress]: <https://docs.silabs.com/gecko-os/1/bgx/latest/getting-started>
