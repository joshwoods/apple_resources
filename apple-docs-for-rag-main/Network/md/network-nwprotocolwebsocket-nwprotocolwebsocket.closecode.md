

- Network
- NWProtocolWebSocket
-  NWProtocolWebSocket.CloseCode 

Enumeration

# NWProtocolWebSocket.CloseCode

Types of codes used upon closing a WebSocket connection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum CloseCode
```

## Topics

### Close Code Types

init(rawValue: UInt16) throws

Initializes a close code with a raw value.

case protocolCode(NWProtocolWebSocket.CloseCode.Defined)

A well-known close code reserved by the protocol (values 1000-2999).

enum Defined

Well-known close code values.

case applicationCode(UInt16)

A close code in the range reserved for applications and frameworks (3000-3999).

case privateCode(UInt16)

A close code in the private-use range (4000-4999).

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Sending Messages

init(opcode: NWProtocolWebSocket.Opcode)

Initializes a WebSocket message with a specific type code.

enum Opcode

Types of messages that you send and receive on a WebSocket connection.

func setPongHandler(DispatchQueue, handler: (NWError?) -> Void)

Sets a handler on a Ping message to be invoked when the corresponding Pong message is received.

var closeCode: NWProtocolWebSocket.CloseCode

The close code on a WebSocket message.

