

- Virtualization
-  VZBridgedNetworkInterface 

Class

# VZBridgedNetworkInterface

An object that identifies the supported network interfaces of the host computer.

macOS 11.0+

``` source
class VZBridgedNetworkInterface
```

## Overview

Use a VZBridgedNetworkInterface object to retrieve the physical interfaces on the host computer. Use a bridged network interface to create a VZBridgedNetworkDeviceAttachment object, which maps that interface to one of your virtual machine’s network devices. The host computer and your virtual machine share access to the physical network interface, but communicate over it using distinct network layers.

You don’t create VZBridgedNetworkInterface objects directly. Instead, the system creates one object for each physical interface of the host computer and stores those objects in the networkInterfaces property. Iterate over the objects in that property to retrieve the network interfaces you need.

## Topics

### Getting the available interfaces

class var networkInterfaces: [VZBridgedNetworkInterface]

The bridged network interfaces that you may use in your virtual machine.

### Getting the interface description

var identifier: String

The unique BSD name of this network interface.

var localizedDisplayName: String?

A user-visible name for the network interface.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

