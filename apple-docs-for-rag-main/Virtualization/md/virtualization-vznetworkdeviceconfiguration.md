

- Virtualization
-  VZNetworkDeviceConfiguration 

Class

# VZNetworkDeviceConfiguration

The common configuration traits for network devices.

macOS 11.0+

``` source
class VZNetworkDeviceConfiguration
```

## Overview

Don’t instantiate the VZNetworkDeviceConfiguration class directly. Instead, instantiate one of its subclasses, such as VZVirtioNetworkDeviceConfiguration. Then use the properties of this class to configure the network device.

## Topics

### Setting configuration attributes

var attachment: VZNetworkDeviceAttachment?

The object that defines how the virtual network device communicates with the host system.

var macAddress: VZMACAddress

The media access control (MAC) address to assign to the network device.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioNetworkDeviceConfiguration

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

class VZVirtioNetworkDeviceConfiguration

A configuration object that requests the creation of a network device for the guest system.

class VZMACAddress

The media access control (MAC) address for a network interface in your virtual machine.

