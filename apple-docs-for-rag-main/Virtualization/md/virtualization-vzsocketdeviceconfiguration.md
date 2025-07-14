

- Virtualization
-  VZSocketDeviceConfiguration 

Class

# VZSocketDeviceConfiguration

The common configuration traits for socket device requests.

macOS 11.0+

``` source
class VZSocketDeviceConfiguration
```

## Overview

Don’t create a VZSocketDeviceConfiguration object directly. Instead, create a VZVirtioSocketDeviceConfiguration object and add it to your virtual machine’s configuration.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioSocketDeviceConfiguration

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

class VZVirtioSocketDeviceConfiguration

A configuration object that requests the creation of a socket device to communicate with the guest system.

