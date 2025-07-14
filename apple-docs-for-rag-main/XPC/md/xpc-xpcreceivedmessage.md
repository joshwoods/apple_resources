

- XPC
-  XPCReceivedMessage 

Structure

# XPCReceivedMessage

A type that represents a message sent between a session and a listener.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
struct XPCReceivedMessage
```

## Mentioned in 

Creating XPC services

## Topics

### Accessing message content

func decode&lt;T>(as: T.Type) throws -> T

Decodes a message as the given type.

var isSync: Bool

A Boolean value that indicates if this message is from a synchronous request.

### Replying to messages

var expectsReply: Bool

A Boolean value that indicates if the client that sent the message expects a reply.

func reply&lt;Message>(Message)

Sends a reply to the originator of the message.

func handoffReply(to: DispatchQueue, () -> Void) -> (any Encodable)?

Informs the system when message processing and response continues in a separate dispatch queue.

## See Also

### Interprocess communication

Creating XPC services

Configure a listener, establish a client session, and exchange messages between processes.

class XPCListener

A type that performs tasks for clients across process boundaries.

class XPCSession

A type that sends messages to a server process.

typealias xpc_listener_t

A C type that performs tasks for clients across process boundaries.

typealias xpc_session_t

A C type that sends messages to a server process.

