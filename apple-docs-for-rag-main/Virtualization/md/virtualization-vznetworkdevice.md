

- Virtualization
-  VZNetworkDevice 

Class

# VZNetworkDevice

A base class that represents a network device in a virtual machine.

macOS 12.0+

``` source
class VZNetworkDevice
```

## Overview

Don’t instantiate a VZNetworkDevice directly. When you create a VZVirtualMachineConfiguration instance with a VZVirtualMachineConfiguration the system creates the number of network devices based on the number of VZVirtioNetworkDeviceConfiguration objects you specify in the VM configuration. Before initializing the virtual machine (VM), validate the configuration using validate() to ensure the user’s computer supports the number of network and other devices you’ve specified.  

For many purposes, a single network that uses a Network Address Translation (NAT) attachment and connects the VM to the host computer’s network is sufficient. You can use additional network interfaces for purposes of your own design, such as:

- Bridging several physical interfaces to connect to multiple networks.

- Using the file descriptor attachment to create specialized connections for different purposes.

You access the network devices through the `VZVirtualMachine`.networkDevices property. The network devices map to their respective configurations in a one to one relationship, where index `i` of `VZVirtualMachine.networkDevices` corresponds to the network device configuration at index `i` set on `VZVirtualMachineConfiguration`.networkDevices.

## Topics

### Getting the network attachment point

var attachment: VZNetworkDeviceAttachment?

The network attachment that’s connected to this network device.

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

## See Also

### Related Documentation

class VZNetworkDeviceConfiguration

The common configuration traits for network devices.

vmnet

Connect with network interfaces to read and write packets on guest operating systems.

