

- Virtualization
-  VZNATNetworkDeviceAttachment 

Class

# VZNATNetworkDeviceAttachment

A device that routes network requests through the host computer and performs network address translation on the resulting packets.

macOS 11.0+

``` source
class VZNATNetworkDeviceAttachment
```

## Overview

A VZNATNetworkDeviceAttachment works with the host computer to perform network address translation (NAT) on the guest system’s network packets, and then route those packets to outside networks. Use this attachment to give the guest system indirect access to external networks, instead of direct access through a shared physical network interface.

To configure a network device with a NAT attachment:

1.  Create the VZNATNetworkDeviceAttachment object.

2.  Assign the attachment object to the attachment property of a VZVirtioNetworkDeviceConfiguration object.

3.  Add the VZVirtioNetworkDeviceConfiguration object to the networkDevices property of your VZVirtualMachineConfiguration.

This attachment doesn’t require your app to have the com.apple.vm.networking entitlement.

## Topics

### Creating the Attachment Point

init()

Creates an attachment that performs network address translation on the guest system’s network packets.

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

class VZBridgedNetworkDeviceAttachment

A network device that interacts directly with a physical network interface on the host computer.

class VZFileHandleNetworkDeviceAttachment

A network device that transmits raw network packets and frames using a datagram socket.

class VZNetworkDeviceAttachment

The common behaviors for the network attachment points of your virtual machine.

