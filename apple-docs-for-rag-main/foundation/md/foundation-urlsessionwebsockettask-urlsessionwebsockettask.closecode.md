

- Foundation
- URLSessionWebSocketTask
-  URLSessionWebSocketTask.CloseCode 

Enumeration

# URLSessionWebSocketTask.CloseCode

A code that indicates why a WebSocket connection closed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum CloseCode
```

## Overview

The WebSocket close codes follow the close codes defined in RFC 6455.

## Topics

### Close codes

case abnormalClosure

A reserved code that indicates the connection closed without a close control frame.

case goingAway

A code that indicates an endpoint is going away.

case internalServerError

A code that indicates the server terminated the connection because it encountered an unexpected condition.

case invalid

A code that indicates the connection is still open.

case invalidFramePayloadData

A code that indicates the server terminated the connection because it received data inconsistent with the message’s type.

case mandatoryExtensionMissing

A code that indicates the client terminated the connection because the server didn’t negotiate a required extension.

case messageTooBig

A code that indicates an endpoint is terminating the connection because it received a message too big for it to process.

case noStatusReceived

A reserved code that indicates an endpoint expected a status code and didn’t receive one.

case normalClosure

A code that indicates normal connection closure.

case policyViolation

A code that indicates an endpoint terminated the connection because it received a message that violates its policy.

case protocolError

A code that indicates an endpoint terminated the connection due to a protocol error.

case tlsHandshakeFailure

A reserved code that indicates the connection closed due to the failure to perform a TLS handshake.

case unsupportedData

A code that indicates an endpoint terminated the connection after receiving a type of data it can’t accept.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Closing the connection

func cancel(with: URLSessionWebSocketTask.CloseCode, reason: Data?)

Sends a close frame with the given close code and optional close reason.

var closeCode: URLSessionWebSocketTask.CloseCode

A code that indicates the reason a connection closed.

var closeReason: Data?

A block of data that provides further information about why a connection closed.

