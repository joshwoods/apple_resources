

- Foundation
- SocketPort
-  socket 

Instance Property

# socket

The receiver’s native socket identifier on the platform.

macOS 10.0+

``` source
var socket: SocketNativeHandle { get }
```

## Discussion

In macOS, the native socket identifier is an integer file descriptor.

## See Also

### Getting Information

var address: Data

The receiver’s socket address structure stored inside an NSData object.

var `protocol`: Int32

The protocol that the receiver uses for communication.

var protocolFamily: Int32

The protocol family that the receiver uses for communication.

var socketType: Int32

The receiver’s socket type.

