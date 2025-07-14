

- Bundle Resources
- Entitlements
-  com.apple.developer.driverkit.family.block-storage-device 

Property List Key

# com.apple.developer.driverkit.family.block-storage-device

A Boolean value that indicates whether to match the driver against block storage devices that use custom drivers.

macOS 12.0+

## Details 

Type  

boolean

## Discussion

Add this entitlement to every BlockStorageDeviceDriverKit driver you create. You must request this entitlement from Apple. For information about how to request the entitlement, see System Extensions and DriverKit.

## See Also

### DriverKit family entitlements

DriverKit Audio Family

A Boolean value that indicates whether the device supports audio functionality.

**Key:** com.apple.developer.driverkit.family.audio

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

