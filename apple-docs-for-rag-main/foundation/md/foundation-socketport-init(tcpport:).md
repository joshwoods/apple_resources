

- Foundation
- SocketPort
-  init(tcpPort:) 

Initializer

# init(tcpPort:)

Initializes the receiver as a local TCP/IP socket of type `SOCK_STREAM`, listening on a specified port number.

macOS 10.0+

``` source
convenience init?(tcpPort port: UInt16)
```

## Parameters 

`port`  

The port number for the newly created socket port to listen on. If `port` is 0, the system will assign a port number.

## Return Value

An initialized local TCP/IP socket of type `SOCK_STREAM`, listening on port `port`.

## Discussion

This method creates an IPv4 port, not an IPv6 port.

## See Also

### Creating Instances

convenience init()

Initializes the receiver as a local TCP/IP socket of type `SOCK_STREAM`.

init?(protocolFamily: Int32, socketType: Int32, protocol: Int32, address: Data)

Initializes the receiver as a local socket with the provided arguments.

init?(protocolFamily: Int32, socketType: Int32, protocol: Int32, socket: SocketNativeHandle)

Initializes the receiver with a previously created local socket.

convenience init?(remoteWithTCPPort: UInt16, host: String?)

Initializes the receiver as a TCP/IP socket of type `SOCK_STREAM` that can connect to a remote host on a specified port.

init(remoteWithProtocolFamily: Int32, socketType: Int32, protocol: Int32, address: Data)

Initializes the receiver as a remote socket with the provided arguments.

