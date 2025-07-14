

- Virtualization
-  VZNetworkDeviceAttachment 

Class

# VZNetworkDeviceAttachment

The common behaviors for the network attachment points of your virtual machine.

macOS 11.0+

``` source
class VZNetworkDeviceAttachment
```

## Overview

Don’t create a VZNetworkDeviceAttachment object directly. Instead, instantiate one of its concrete subclasses and use that object to configure your network devices. Each concrete subclass represents a specific type of network interface on the host computer.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZBridgedNetworkDeviceAttachment
- VZFileHandleNetworkDeviceAttachment
- VZNATNetworkDeviceAttachment

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

class VZNATNetworkDeviceAttachment

A device that routes network requests through the host computer and performs network address translation on the resulting packets.

