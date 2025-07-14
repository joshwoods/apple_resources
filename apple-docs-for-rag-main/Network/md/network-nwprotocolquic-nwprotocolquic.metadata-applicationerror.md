

- Network
- NWProtocolQUIC
- NWProtocolQUIC.Metadata
-  applicationError 

Instance Property

# applicationError

The QUIC application error code to send for the connection, or received from the peer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var applicationError: NWProtocolQUIC.ApplicationError { get set }
```

## See Also

### Handling Errors

struct ApplicationError

A QUIC application error code.

var streamApplicationErrorCode: UInt64

The QUIC application error code to send for the stream, or received from the peer.

