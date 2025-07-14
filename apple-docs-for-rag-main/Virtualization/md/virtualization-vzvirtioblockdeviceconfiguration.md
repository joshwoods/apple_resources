

- Virtualization
-  VZVirtioBlockDeviceConfiguration 

Class

# VZVirtioBlockDeviceConfiguration

The configuration object that requests the creation of a virtual storage device in the guest system.

macOS 11.0+

``` source
class VZVirtioBlockDeviceConfiguration
```

## Overview

Use a VZVirtioBlockDeviceConfiguration object to create an emulated storage device in your virtual machine. When you add this object to your virtual machine configuration, the virtual machine creates an emulated disk for the guest operating system to use to read and write files. The emulated storage device conforms to the Virtio Block Device specification.

When you create a VZVirtioBlockDeviceConfiguration object, specify the attachment object that implements the underlying storage. For example, specify a VZDiskImageStorageDeviceAttachment object to configure the storage device using a disk image in the local file system. Assign your configuration object to the storageDevices property of your VZVirtualMachineConfiguration object before creating your virtual machine.

## Topics

### Creating the configuration object

init(attachment: VZStorageDeviceAttachment)

Creates a block device configuration object that uses the specified storage medium.

### Identifying a block device

var blockDeviceIdentifier: String

The string that identifies the VIRTIO block device.

### Validating device identifiers

class func validateBlockDeviceIdentifier(String) throws

Checks the validity of a block device identifier.

## Relationships

### Inherits From

- VZStorageDeviceConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configurations

class VZStorageDeviceConfiguration

The common configuration traits for storage device requests.

class VZUSBMassStorageDeviceConfiguration

The configuration object that represents a USB Mass storage device.

enum VZDiskImageCachingMode

An integer that describes the disk image caching mode.

enum VZDiskImageSynchronizationMode

An integer that describes the disk image synchronization mode.

class VZNVMExpressControllerDeviceConfiguration

The configuration object that represents an NVM Express Controller storage device.

