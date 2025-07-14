

- Foundation
- SocketPort
-  init() 

Initializer

# init()

Initializes the receiver as a local TCP/IP socket of type `SOCK_STREAM`.

macOS 10.0+

``` source
convenience init()
```

## Return Value

An initialized local TCP/IP socket port of type `SOCK_STREAM`.

## Discussion

The port number is selected by the system.

## See Also

### Related Documentation

Distributed Objects Programming Topics

### Creating Instances

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

