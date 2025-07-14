

- Foundation
- URLSessionWebSocketTask
- URLSessionWebSocketTask.CloseCode
-  URLSessionWebSocketTask.CloseCode.goingAway 

Case

# URLSessionWebSocketTask.CloseCode.goingAway

A code that indicates an endpoint is going away.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case goingAway
```

## Discussion

This code indicates situations like a server going down or a browser having navigated away from a page.

## See Also

### Close codes

case abnormalClosure

A reserved code that indicates the connection closed without a close control frame.

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

