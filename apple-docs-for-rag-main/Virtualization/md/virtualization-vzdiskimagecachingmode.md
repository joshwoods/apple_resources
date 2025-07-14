

- Virtualization
-  VZDiskImageCachingMode 

Enumeration

# VZDiskImageCachingMode

An integer that describes the disk image caching mode.

macOS 12.0+

``` source
enum VZDiskImageCachingMode
```

## Topics

### Disk image caching modes

case automatic

Allows the virtualization framework to automatically determine whether to enable data caching.

case cached

Enables data caching.

case uncached

Disables data caching.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configurations

class VZVirtioBlockDeviceConfiguration

The configuration object that requests the creation of a virtual storage device in the guest system.

class VZStorageDeviceConfiguration

The common configuration traits for storage device requests.

class VZUSBMassStorageDeviceConfiguration

The configuration object that represents a USB Mass storage device.

enum VZDiskImageSynchronizationMode

An integer that describes the disk image synchronization mode.

class VZNVMExpressControllerDeviceConfiguration

The configuration object that represents an NVM Express Controller storage device.

