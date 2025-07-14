

- Virtualization
-  VZDirectorySharingDevice 

Class

# VZDirectorySharingDevice

The base class that represents a directory sharing device in a VM.

macOS 12.0+

``` source
class VZDirectorySharingDevice
```

## Overview

Don’t instantiate `VZDirectorySharingDevice` directly; configure a directory sharing device first by using VZVirtualMachineConfiguration through a subclass of VZDirectorySharingDeviceConfiguration.

When you create a VZVirtualMachine from the configuration, the directory sharing devices are available through the `VZVirtualMachine.directorySharingDevices` property.

The real type of `VZDirectorySharingDevice` corresponds to the type used by the configuration. For example, a VZVirtioFileSystemDeviceConfiguration leads to a device of type VZVirtioFileSystemDevice.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioFileSystemDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Shared directory devices

class VZVirtioFileSystemDevice

An object the defines a VIRTIO file system device.

