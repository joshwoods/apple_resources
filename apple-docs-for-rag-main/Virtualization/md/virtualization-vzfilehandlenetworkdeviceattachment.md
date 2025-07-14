

- Virtualization
-  VZFileHandleNetworkDeviceAttachment 

Class

# VZFileHandleNetworkDeviceAttachment

A network device that transmits raw network packets and frames using a datagram socket.

macOS 11.0+

``` source
class VZFileHandleNetworkDeviceAttachment
```

## Overview

A VZFileHandleNetworkDeviceAttachment object maps a network interface to a connected datagram socket. This attachment transmits data at the data link layer. You configure and manage the socket in your app, and manage the corresponding data transfers.

To configure a network device with a socket-based file handle:

1.  Create a socket with the `SOCK_DGRAM` type in your app.

2.  Create a FileHandle from the socket’s file descriptor.

3.  Create the VZFileHandleNetworkDeviceAttachment object using the file handle.

4.  Assign the attachment object to the attachment property of a VZVirtioNetworkDeviceConfiguration object.

5.  Add the VZVirtioNetworkDeviceConfiguration object to the networkDevices property of your VZVirtualMachineConfiguration.

This attachment doesn’t require your app to have the com.apple.vm.networking entitlement.

## Topics

### Creating the attachment point

init(fileHandle: FileHandle)

Creates the attachment from a file handle that contains a connected datagram socket.

### Getting the file handle

var fileHandle: FileHandle

The file handle assigned to this attachment.

### Specifying the network packet size

var maximumTransmissionUnit: Int

An integer value that indicates the maximum transmission unit (MTU) associated with this attachment.

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

class VZNATNetworkDeviceAttachment

A device that routes network requests through the host computer and performs network address translation on the resulting packets.

class VZNetworkDeviceAttachment

The common behaviors for the network attachment points of your virtual machine.

