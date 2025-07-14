

- Network
- NWProtocolWebSocket
- NWProtocolWebSocket.CloseCode
-  NWProtocolWebSocket.CloseCode.privateCode(\_:) 

Case

# NWProtocolWebSocket.CloseCode.privateCode(\_:)

A close code in the private-use range (4000-4999).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case privateCode(UInt16)
```

## See Also

### Close Code Types

init(rawValue: UInt16) throws

Initializes a close code with a raw value.

case protocolCode(NWProtocolWebSocket.CloseCode.Defined)

A well-known close code reserved by the protocol (values 1000-2999).

enum Defined

Well-known close code values.

case applicationCode(UInt16)

A close code in the range reserved for applications and frameworks (3000-3999).

