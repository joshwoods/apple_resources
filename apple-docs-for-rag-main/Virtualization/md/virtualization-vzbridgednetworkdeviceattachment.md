

- Virtualization
-  VZBridgedNetworkDeviceAttachment 

Class

# VZBridgedNetworkDeviceAttachment

A network device that interacts directly with a physical network interface on the host computer.

macOS 11.0+

``` source
class VZBridgedNetworkDeviceAttachment
```

## Overview

A VZBridgedNetworkDeviceAttachment object represents a physical interface on the host computer. Use this object when configuring a network interface for your virtual machine. A bridged network device sends and receives packets on the same physical interface as the host computer, but does so using a different network layer.

Important

To use this attachment, your app must have the com.apple.vm.networking entitlement. If it doesn’t, the use of this attachment point results in an invalid VZVirtualMachineConfiguration object.

To configure a network device with a bridged network interface:

1.  Obtain a reference to one of the host’s physical network interfaces from the networkInterfaces property of VZBridgedNetworkInterface.

2.  Create the VZBridgedNetworkDeviceAttachment object using the network interface.

3.  Assign the attachment object to the attachment property of a VZVirtioNetworkDeviceConfiguration object.

4.  Add the VZVirtioNetworkDeviceConfiguration object to the networkDevices property of your VZVirtualMachineConfiguration.

## Topics

### Creating the attachment point

init(interface: VZBridgedNetworkInterface)

Creates the attachment from a bridged network interface object.

### Getting the network interface

var interface: VZBridgedNetworkInterface

The network interface assigned to this attachment.

## Relationships

### Inherits From

- VZNetworkDeviceAttachment

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Attachment points

class VZFileHandleNetworkDeviceAttachment

A network device that transmits raw network packets and frames using a datagram socket.

class VZNATNetworkDeviceAttachment

A device that routes network requests through the host computer and performs network address translation on the resulting packets.

class VZNetworkDeviceAttachment

The common behaviors for the network attachment points of your virtual machine.

