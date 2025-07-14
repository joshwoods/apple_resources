

- Virtualization
-  VZVirtioSocketConnection 

Class

# VZVirtioSocketConnection

A port-based connection between the guest operating system and the host computer.

macOS 11.0+

``` source
class VZVirtioSocketConnection
```

## Overview

A VZVirtioSocketConnection object contains the port information for the guest operating system and host computer. You don’t create connection objects directly. When the guest operating system initiates a connection, the virtual machine creates the connection object and passes it to the appropriate VZVirtioSocketListener object, which forwards the object to its delegate. When the virtual machine opens a connection to a guest port, the connect(toPort:) method (Objective-C) or connect(toPort:completionHandler:) method (Swift) pass the connection object to your completion handler.

## Topics

### Getting the connection details

var sourcePort: UInt32

The port number of the system that opened the connection.

var destinationPort: UInt32

The destination port number of the connection.

var fileDescriptor: Int32

The file descriptor to use when sending data.

### Closing the connection

func close()

Close the file descriptor associated with the socket.

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

### Connection management

class VZVirtioSocketListener

An object that listens for port-based connection requests from the guest operating system.

