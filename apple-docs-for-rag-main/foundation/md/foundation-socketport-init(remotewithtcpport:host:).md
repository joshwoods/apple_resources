

- Foundation
- SocketPort
-  init(remoteWithTCPPort:host:) 

Initializer

# init(remoteWithTCPPort:host:)

Initializes the receiver as a TCP/IP socket of type `SOCK_STREAM` that can connect to a remote host on a specified port.

macOS 10.0+

``` source
convenience init?(
    remoteWithTCPPort port: UInt16,
    host hostName: String?
)
```

## Parameters 

`port`  

The port to connect to.

`hostName`  

The host name to connect to. `hostName` may be either a host name or an IPv4-style address.

## Return Value

A TCP/IP socket port of type `SOCK_STREAM` that can connect to the remote host `hostName` on port `port`.

## Discussion

A connection is not opened to the remote host until data is sent.

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

init(remoteWithProtocolFamily: Int32, socketType: Int32, protocol: Int32, address: Data)

Initializes the receiver as a remote socket with the provided arguments.

