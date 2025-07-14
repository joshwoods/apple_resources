

- Foundation
-  SocketPort 

Class

# SocketPort

A port that represents a BSD socket.

macOS 10.0+

``` source
class SocketPort
```

## Overview

A SocketPort object can be used as an endpoint for distributed object connections. Companion classes, NSMachPort and MessagePort, allow for local (on the same machine) communication only. The SocketPort class allows for both local and remote communication, but may be more expensive than the others for the local case.

Note

The SocketPort class conforms to the NSCoding protocol, but only supports coding by an NSPortCoder. Port and its other subclasses do not support archiving.

## Topics

### Creating Instances

convenience init()

Initializes the receiver as a local TCP/IP socket of type `SOCK_STREAM`.

convenience init?(tcpPort: UInt16)

Initializes the receiver as a local TCP/IP socket of type `SOCK_STREAM`, listening on a specified port number.

init?(protocolFamily: Int32, socketType: Int32, protocol: Int32, address: Data)

Initializes the receiver as a local socket with the provided arguments.

init?(protocolFamily: Int32, socketType: Int32, protocol: Int32, socket: SocketNativeHandle)

Initializes the receiver with a previously created local socket.

convenience init?(remoteWithTCPPort: UInt16, host: String?)

Initializes the receiver as a TCP/IP socket of type `SOCK_STREAM` that can connect to a remote host on a specified port.

init(remoteWithProtocolFamily: Int32, socketType: Int32, protocol: Int32, address: Data)

Initializes the receiver as a remote socket with the provided arguments.

### Getting Information

var address: Data

The receiver’s socket address structure stored inside an NSData object.

var `protocol`: Int32

The protocol that the receiver uses for communication.

var protocolFamily: Int32

The protocol family that the receiver uses for communication.

var socket: SocketNativeHandle

The receiver’s native socket identifier on the platform.

var socketType: Int32

The receiver’s socket type.

## Relationships

### Inherits From

- Port

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Sockets

class Host

A representation of an individual host on the network.

Deprecated

class Port

An abstract class that represents a communication channel.

