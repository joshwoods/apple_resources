

- Foundation
- SocketPort
-  init(protocolFamily:socketType:protocol:socket:) 

Initializer

# init(protocolFamily:socketType:protocol:socket:)

Initializes the receiver with a previously created local socket.

macOS 10.0+

``` source
init?(
    protocolFamily family: Int32,
    socketType type: Int32,
    protocol: Int32,
    socket sock: SocketNativeHandle
)
```

## Parameters 

`family`  

The protocol family for the provided socket. Possible values are defined in ``, such as `AF_LOCAL`, `AF_INET`, and `AF_INET6`.

`type`  

The type of the provided socket.

`protocol`  

The specific protocol the provided socket uses.

`sock`  

The previously created socket.

## Return Value

A local socket port initialized with the provided socket.

## See Also

### Creating Instances

convenience init()

Initializes the receiver as a local TCP/IP socket of type `SOCK_STREAM`.

convenience init?(tcpPort: UInt16)

Initializes the receiver as a local TCP/IP socket of type `SOCK_STREAM`, listening on a specified port number.

init?(protocolFamily: Int32, socketType: Int32, protocol: Int32, address: Data)

Initializes the receiver as a local socket with the provided arguments.

convenience init?(remoteWithTCPPort: UInt16, host: String?)

Initializes the receiver as a TCP/IP socket of type `SOCK_STREAM` that can connect to a remote host on a specified port.

init(remoteWithProtocolFamily: Int32, socketType: Int32, protocol: Int32, address: Data)

Initializes the receiver as a remote socket with the provided arguments.

