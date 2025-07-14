

- Foundation
- SocketPort
-  protocolFamily 

Instance Property

# protocolFamily

The protocol family that the receiver uses for communication.

macOS 10.0+

``` source
var protocolFamily: Int32 { get }
```

## Discussion

Possible values are defined in ``, such as `AF_LOCAL`, `AF_INET`, and `AF_INET6`.

## See Also

### Getting Information

var address: Data

The receiver’s socket address structure stored inside an NSData object.

var `protocol`: Int32

The protocol that the receiver uses for communication.

var socket: SocketNativeHandle

The receiver’s native socket identifier on the platform.

var socketType: Int32

The receiver’s socket type.

