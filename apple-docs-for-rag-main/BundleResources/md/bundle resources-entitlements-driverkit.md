

- Bundle Resources
- Entitlements
-  DriverKit 

API Collection

# DriverKit

Develop device drivers in macOS and iPadOS.

## Topics

### Essentials

com.apple.developer.driverkit

A Boolean value that indicates whether your extension has permission to run as a user-space driver.

### DriverKit family entitlements

DriverKit Audio Family

A Boolean value that indicates whether the device supports audio functionality.

**Key:** com.apple.developer.driverkit.family.audio

com.apple.developer.driverkit.family.block-storage-device

A Boolean value that indicates whether to match the driver against block storage devices that use custom drivers.

com.apple.developer.driverkit.family.midi

A Boolean value that indicates whether to match the driver against devices that support MIDI.

com.apple.developer.driverkit.family.networking

A Boolean value that indicates whether to match the driver against devices that communicate using networking protocols.

com.apple.developer.driverkit.family.scsicontroller

A Boolean value that indicates whether to match the driver against devices with SCSI controllers.

com.apple.developer.driverkit.family.serial

A Boolean value that indicates whether to match the driver against devices with serial communication interfaces.

com.apple.developer.driverkit.transport.pci

An array of PCI device descriptors that your custom driver supports.

com.apple.developer.driverkit.transport.usb

An array of dictionaries that identify the USB devices the driver supports.

### User client entitlements

com.apple.developer.driverkit.userclient-access

An array of strings that represent macOS driver extensions that may communicate with other DriverKit services.

com.apple.developer.driverkit.allow-any-userclient-access

A Boolean value that determines whether a macOS driver accepts user client connections from any application.

Communicates with Drivers

A Boolean value that indicates whether an iPadOS app can communicate with drivers.

**Key:** com.apple.developer.driverkit.communicates-with-drivers

DriverKit Allow Third Party User Clients

A Boolean value that indicates whether an iPadOS driver accepts calls from third-party user clients.

**Key:** com.apple.developer.driverkit.allow-third-party-userclients

## See Also

### System

System Extensions

Extend the capabilities of macOS from user space.

