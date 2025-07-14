

- Virtualization
-  VZStorageDeviceConfiguration 

Class

# VZStorageDeviceConfiguration

The common configuration traits for storage device requests.

macOS 11.0+

``` source
class VZStorageDeviceConfiguration
```

## Overview

Don’t create a VZStorageDeviceConfiguration object directly. Instead, instantiate one of its subclasses, such as VZVirtioBlockDeviceConfiguration. Use the attachment property of this class to access the device’s underlying storage.

## Topics

### Getting the attachment point

var attachment: VZStorageDeviceAttachment

The attachment object that provides the underlying storage for the device.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZNVMExpressControllerDeviceConfiguration
- VZUSBMassStorageDeviceConfiguration
- VZVirtioBlockDeviceConfiguration

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

class VZVirtioBlockDeviceConfiguration

The configuration object that requests the creation of a virtual storage device in the guest system.

class VZUSBMassStorageDeviceConfiguration

The configuration object that represents a USB Mass storage device.

enum VZDiskImageCachingMode

An integer that describes the disk image caching mode.

enum VZDiskImageSynchronizationMode

An integer that describes the disk image synchronization mode.

class VZNVMExpressControllerDeviceConfiguration

The configuration object that represents an NVM Express Controller storage device.

