

- Virtualization
-  VZUSBMassStorageDeviceConfiguration 

Class

# VZUSBMassStorageDeviceConfiguration

The configuration object that represents a USB Mass storage device.

macOS 13.0+

``` source
class VZUSBMassStorageDeviceConfiguration
```

## Topics

### Creating the configuration object

init(attachment: VZStorageDeviceAttachment)

Creates a new storage device configuration with the specified attachment.

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
- VZUSBDeviceConfiguration

## See Also

### Configurations

class VZVirtioBlockDeviceConfiguration

The configuration object that requests the creation of a virtual storage device in the guest system.

class VZStorageDeviceConfiguration

The common configuration traits for storage device requests.

enum VZDiskImageCachingMode

An integer that describes the disk image caching mode.

enum VZDiskImageSynchronizationMode

An integer that describes the disk image synchronization mode.

class VZNVMExpressControllerDeviceConfiguration

The configuration object that represents an NVM Express Controller storage device.

