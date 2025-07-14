

- Virtualization
-  VZMACAddress 

Class

# VZMACAddress

The media access control (MAC) address for a network interface in your virtual machine.

macOS 11.0+

``` source
class VZMACAddress
```

## Overview

A VZMACAddress object contains the hardware address of your network interface. Every network device has a unique 48-bit MAC address that the system uses to route network packets to that device.

Call the randomLocallyAdministered() method to get a local MAC address suitable for use with your network interfaces. Alternatively, you can create a VZMACAddress object yourself from a string or `ether_addr_t` structure.

## Topics

### Creating a MAC address

class func randomLocallyAdministered() -> Self

Returns a valid, random, locally administered, unicast MAC address.

convenience init?(string: String)

Creates a MAC address object from a specially formatted string.

init(ethernetAddress: ether_addr_t)

Creates a MAC address from the specified 48-bit Ethernet address.

### Getting the address

var string: String

The MAC address as a formatted string.

var ethernetAddress: ether_addr_t

The MAC address as an Ethernet data structure.

### Getting address attributes

var isBroadcastAddress: Bool

A Boolean value that indicates whether the address is a broadcast address.

var isMulticastAddress: Bool

A Boolean value that indicates whether the address is a multicast address.

var isUnicastAddress: Bool

A Boolean value that indicates whether the address is a unicast address.

var isLocallyAdministeredAddress: Bool

A Boolean value that indicates whether the address is a locally administered address (LAA).

var isUniversallyAdministeredAddress: Bool

A Boolean value that indicates whether the address is a universally adminstered address (UAA).

## Relationships

### Inherits From

- NSObject

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

class VZNetworkDeviceConfiguration

The common configuration traits for network devices.

