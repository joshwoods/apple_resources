

- Virtualization
-  VZNVMExpressControllerDeviceConfiguration 

Class

# VZNVMExpressControllerDeviceConfiguration

The configuration object that represents an NVM Express Controller storage device.

macOS 14.0+

``` source
class VZNVMExpressControllerDeviceConfiguration
```

## Overview

This device configuration creates a storage device that conforms to the NVM Express specification revision 1.1b.

The device configuration is valid only if used with VZGenericPlatformConfiguration.

## Topics

### Creating a new device configuration

init(attachment: VZStorageDeviceAttachment)

Creates a new NVM Express controller configuration with the storage device attachment you provide.

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

### Related Documentation

class VZGenericPlatformConfiguration

The platform configuration for a generic Intel or ARM virtual machine.

### Configurations

class VZVirtioBlockDeviceConfiguration

The configuration object that requests the creation of a virtual storage device in the guest system.

class VZStorageDeviceConfiguration

The common configuration traits for storage device requests.

class VZUSBMassStorageDeviceConfiguration

The configuration object that represents a USB Mass storage device.

enum VZDiskImageCachingMode

An integer that describes the disk image caching mode.

enum VZDiskImageSynchronizationMode

An integer that describes the disk image synchronization mode.

