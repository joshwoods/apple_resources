

- Virtualization
-  VZVirtioSocketDeviceConfiguration 

Class

# VZVirtioSocketDeviceConfiguration

A configuration object that requests the creation of a socket device to communicate with the guest system.

macOS 11.0+

``` source
class VZVirtioSocketDeviceConfiguration
```

## Overview

Use a VZVirtioSocketDeviceConfiguration object to implement port-based communication between the guest operating system and the host computer. When you add this object to the socketDevices property of your VZVirtualMachineConfiguration, the virtual machine provides a corresponding VZVirtioSocketDevice object to use to configure the ports. Add only one VZVirtioSocketDeviceConfiguration to your virtual machine’s configuration.

## Topics

### Creating the Configuration Object

init()

Creates a socket device configuration object.

## Relationships

### Inherits From

- VZSocketDeviceConfiguration

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

class VZSocketDeviceConfiguration

The common configuration traits for socket device requests.

