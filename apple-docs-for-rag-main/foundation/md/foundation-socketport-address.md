

- Foundation
- SocketPort
-  address 

Instance Property

# address

The receiver’s socket address structure stored inside an NSData object.

macOS 10.0+

``` source
var address: Data { get }
```

## See Also

### Related Documentation

init(remoteWithProtocolFamily: Int32, socketType: Int32, protocol: Int32, address: Data)

Initializes the receiver as a remote socket with the provided arguments.

init?(protocolFamily: Int32, socketType: Int32, protocol: Int32, address: Data)

Initializes the receiver as a local socket with the provided arguments.

### Getting Information

var `protocol`: Int32

The protocol that the receiver uses for communication.

var protocolFamily: Int32

The protocol family that the receiver uses for communication.

var socket: SocketNativeHandle

The receiver’s native socket identifier on the platform.

var socketType: Int32

The receiver’s socket type.

