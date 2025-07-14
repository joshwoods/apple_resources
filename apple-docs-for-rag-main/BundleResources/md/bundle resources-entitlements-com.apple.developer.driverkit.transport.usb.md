

- Bundle Resources
- Entitlements
-  com.apple.developer.driverkit.transport.usb 

Property List Key

# com.apple.developer.driverkit.transport.usb

An array of dictionaries that identify the USB devices the driver supports.

macOS 10.15+

## Details 

Type  

array of dictionaries

## Discussion

Each element in the array is a dictionary whose keys and values identify a specific type of supported device. The keys in the dictionary correspond to field names of the device descriptor associated with the USB device.

## Topics

### Property List Keys

bConfigurationValue

bDeviceClass

bDeviceProtocol

bDeviceSubClass

bInterfaceClass

bInterfaceNumber

bInterfaceProtocol

bInterfaceSubClass

bcdDevice

idProduct

idProductArray

idProductMask

idVendor

## See Also

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

