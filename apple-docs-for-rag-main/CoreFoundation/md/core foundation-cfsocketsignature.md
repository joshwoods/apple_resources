

- Core Foundation
-  CFSocketSignature 

Structure

# CFSocketSignature

A structure that fully specifies the communication protocol and connection address of a CFSocket object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFSocketSignature
```

## Topics

### Initializers

init()

init(protocolFamily: Int32, socketType: Int32, protocol: Int32, address: Unmanaged&lt;CFData>!)

### Instance Properties

var address: Unmanaged&lt;CFData>!

A CFData object holding the contents of a `struct sockaddr` appropriate for the given protocol family (`struct sockaddr_in` or `struct sockaddr_in6`, for example), identifying the address of the socket.

var `protocol`: Int32

The protocol type of the socket.

var protocolFamily: Int32

The protocol family of the socket.

var socketType: Int32

The socket type of the socket.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct CFSocketContext

A structure that contains program-defined data and callbacks with which you can configure a CFSocket object’s behavior.

typealias CFSocketNativeHandle

Type for the platform-specific native socket handle.

