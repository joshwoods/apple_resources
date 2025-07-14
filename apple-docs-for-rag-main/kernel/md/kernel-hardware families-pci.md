

- Kernel
- Hardware Families
-  PCI 

API Collection

# PCI

Implement a driver that supports Thunderbolt devices or PCI cards.

## Overview

For many types of PCI drivers, the use of kernel extensions is deprecated. Instead, create a DriverKit extension using PCIDriverKit.

## Topics

### Devices

Implementing a PCIe Kext for a Thunderbolt Device

Create an IOKit driver to support Thunderbolt devices that implement features not supported in PCIDriverKit, such as wireless networking or audio.

IOPCIDevice

An IOService class representing a PCI device.

Deprecated

IOAGPDevice

An IOService class representing an AGP primary device.

Deprecated

### Event Source

IOPCIEventSourceDeprecated

## See Also

### Hardware Interconnects

ATA

Implement a driver that supports Advanced Technology Attachment (ATA) devices.

Bluetooth

Implement a driver that supports Bluetooth devices.

FireWire

Implement a driver that supports FireWire devices.

USB

Implement a driver that supports Universal Serial Bus (USB) devices.

