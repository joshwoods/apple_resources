

- Virtualization
-  VZDiskImageSynchronizationMode 

Enumeration

# VZDiskImageSynchronizationMode

An integer that describes the disk image synchronization mode.

macOS 12.0+

``` source
enum VZDiskImageSynchronizationMode
```

## Topics

### Disk image synchronization modes

case full

Synchronizes data to the permanent storage holding the disk image.

case fsync

Synchronizes data to the drive using the system’s best-effort synchronization mode.

case none

Disables data synchronization with the permanent storage.

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

enum VZDiskImageCachingMode

An integer that describes the disk image caching mode.

class VZNVMExpressControllerDeviceConfiguration

The configuration object that represents an NVM Express Controller storage device.

