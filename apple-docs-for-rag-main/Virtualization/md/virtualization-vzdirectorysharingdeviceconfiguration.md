

- Virtualization
-  VZDirectorySharingDeviceConfiguration 

Class

# VZDirectorySharingDeviceConfiguration

The base class for a directory sharing device configuration.

macOS 12.0+

``` source
class VZDirectorySharingDeviceConfiguration
```

## Overview

Don’t instantiate `VZDirectorySharingDeviceConfiguration` directly. Instead use one of its subclasses, like VZVirtioFileSystemDeviceConfiguration.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioFileSystemDeviceConfiguration

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

class VZVirtioFileSystemDeviceConfiguration

An object that represents the configuration of a Virtio file system device.

class VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

