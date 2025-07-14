

- Virtualization
-  VZVirtioNetworkDeviceConfiguration 

Class

# VZVirtioNetworkDeviceConfiguration

A configuration object that requests the creation of a network device for the guest system.

macOS 11.0+

``` source
class VZVirtioNetworkDeviceConfiguration
```

## Mentioned in 

Creating and Running a Linux Virtual Machine

## Overview

Use a VZVirtioNetworkDeviceConfiguration object to configure one network interface of your virtual machine. After creating this object, assign an appropriate value to its inherited attachment property to define the type of network interface you want. You can also assign a specific MAC address, or let the system generate a random address for you.

After creating and configuring a VZVirtioNetworkDeviceConfiguration object, assign it to the networkDevices property of your virtual machine’s configuration.

## Topics

### Creating the configuration object

init()

Creates a network device configuration object for you to configure.

## Relationships

### Inherits From

- VZNetworkDeviceConfiguration

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

class VZNetworkDeviceConfiguration

The common configuration traits for network devices.

class VZMACAddress

The media access control (MAC) address for a network interface in your virtual machine.

