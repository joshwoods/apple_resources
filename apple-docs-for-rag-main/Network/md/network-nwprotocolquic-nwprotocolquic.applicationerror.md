

- Network
- NWProtocolQUIC
-  NWProtocolQUIC.ApplicationError 

Structure

# NWProtocolQUIC.ApplicationError

A QUIC application error code.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ApplicationError
```

## Topics

### Configuring Application Errors

init(code: UInt64, reason: String?)

Initializes a QUIC application error with an error code and an optional reason.

### Inspecting Application Errors

let code: UInt64

The QUIC application error code.

let reason: String?

The QUIC application error reason.

## Relationships

### Conforms To

- ExpressibleByIntegerLiteral
- Sendable

## See Also

### Handling Errors

var applicationError: NWProtocolQUIC.ApplicationError

The QUIC application error code to send for the connection, or received from the peer.

var streamApplicationErrorCode: UInt64

The QUIC application error code to send for the stream, or received from the peer.

