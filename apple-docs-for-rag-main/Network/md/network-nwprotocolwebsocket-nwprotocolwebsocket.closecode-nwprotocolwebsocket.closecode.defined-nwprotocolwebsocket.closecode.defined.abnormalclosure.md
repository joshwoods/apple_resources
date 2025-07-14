

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.CloseCode
- NWProtocolWebSocket.CloseCode.Defined
-  NWProtocolWebSocket.CloseCode.Defined.abnormalClosure 

Case

# NWProtocolWebSocket.CloseCode.Defined.abnormalClosure

This value is reserved for local errors and indicates that no Close message was received.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case abnormalClosure
```

## See Also

### Defined Close Codes

case normalClosure

A normal closure occurred with no errors.

case goingAway

An endpoint is no longer available, such as when a server is down.

case protocolError

An endpoint is terminating the connection due to a protocol error.

case unsupportedData

An endpoint is terminating the connection because it received a type of data it cannot accept.

case noStatusReceived

This value is reserved for local errors and indicates that no Close code was received.

case invalidFramePayloadData

An endpoint is terminating the connection because it received data within a message that was inconsistent with the message type.

case policyViolation

An endpoint is terminating the connection because it received a message that violates its policy.

case messageTooBig

An endpoint is terminating the connection because it received a message that is too big for it to process.

case mandatoryExtension

The WebSocket client expected the server to negotiate one or more extensions that were not negotiated.

case internalServerError

The server is terminating the connection because it encountered an unexpected condition that prevented it from fulfilling the request.

case tlsHandshake

This value is reserved for local errors and indicates that the TLS handshake failed.

