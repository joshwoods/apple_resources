

- Virtualization
-  VZMemoryBalloonDevice 

Class

# VZMemoryBalloonDevice

The common behavior for memory devices.

macOS 11.0+

``` source
class VZMemoryBalloonDevice
```

## Overview

Don’t instantiate this class directly. To request a memory ballon device, add an appropriate configuration object to the memoryBalloonDevices property of the VZVirtualMachineConfiguration object that you use to configure the virtual machine. In response, the system instantiates the subclass of VZMemoryBalloonDevice that matches your request. For example, if you supply a VZVirtioTraditionalMemoryBalloonDeviceConfiguration object in your configuration, the system creates a VZVirtioTraditionalMemoryBalloonDevice object.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioTraditionalMemoryBalloonDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Memory balloon devices

class VZVirtioTraditionalMemoryBalloonDevice

The object you use to change the amount of memory allocated to the guest system.

