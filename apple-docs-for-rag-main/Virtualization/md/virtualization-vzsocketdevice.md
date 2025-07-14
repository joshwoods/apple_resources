

- Virtualization
-  VZSocketDevice 

Class

# VZSocketDevice

The common behavior of socket devices.

macOS 11.0+

``` source
class VZSocketDevice
```

## Overview

Don’t create or use a VZSocketDevice object directly. If your virtual machine’s configuration includes a VZVirtioSocketDeviceConfiguration object, the virtual machine returns a VZVirtioSocketDevice object in its socketDevices property. Use that object to configure the port-based communications for your virtual machine.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioSocketDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Devices

class VZVirtioSocketDevice

A device that manages port-based connections between the guest system and the host computer.

