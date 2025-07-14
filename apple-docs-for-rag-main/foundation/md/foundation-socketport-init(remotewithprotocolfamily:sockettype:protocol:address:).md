

- Foundation
- SocketPort
-  init(remoteWithProtocolFamily:socketType:protocol:address:) 

Initializer

# init(remoteWithProtocolFamily:socketType:protocol:address:)

Initializes the receiver as a remote socket with the provided arguments.

macOS 10.0+

``` source
init(
    remoteWithProtocolFamily family: Int32,
    socketType type: Int32,
    protocol: Int32,
    address: Data
)
```

## Parameters 

`family`  

The protocol family for the socket port. Possible values are defined in ``, such as `AF_LOCAL`, `AF_INET`, and `AF_INET6`.

`type`  

The type of socket.

`protocol`  

The specific protocol to use from the protocol family.

`address`  

The family-specific socket address for the receiver copied into an `NSData` object.

## Discussion

A connection is not opened to the remote address until data is sent.

## See Also

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

