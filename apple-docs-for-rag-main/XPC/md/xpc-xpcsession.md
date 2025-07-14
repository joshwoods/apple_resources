

- XPC
-  XPCSession 

Class

# XPCSession

A type that sends messages to a server process.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
class XPCSession
```

## Overview

XPC sessions are stateful connections you use to send structured messages to a separate process. Once established, a session remains active until one side of the connection cancels it, at which point the system invalidates the connection.

## Topics

### Creating a session

convenience init&lt;Message>(xpcService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((Message) -> (any Encodable)?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to an XPC service with the name and decodable message handler you specify.

convenience init(xpcService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((XPCReceivedMessage) -> (any Encodable)?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to an XPC service with the name and received message handler you specify.

convenience init(xpcService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((XPCDictionary) -> XPCDictionary?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to an XPC service with the name and dictionary message handler you specify.

convenience init(xpcService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to an XPC service with the name you specify.

convenience init&lt;Message>(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((Message) -> (any Encodable)?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name and decodable message handler you specify.

convenience init(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((XPCReceivedMessage) -> (any Encodable)?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name and received message handler you specify.

convenience init(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((XPCDictionary) -> XPCDictionary?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name and dictionary message handler you specify.

convenience init(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name you specify.

struct InitializationOptions

Options that control the session’s configuration.

func setTargetQueue(DispatchQueue)

Sets the target dispatch queue on an inactive session for processing messages.

### Managing the life cycle

func activate() throws

Activates a session so you can send messages.

func setIncomingMessageHandler&lt;Message>((Message) -> (any Encodable)?)

Sets a closure to receive incoming decodable messages for a session.

func setIncomingMessageHandler((XPCReceivedMessage) -> (any Encodable)?)

Sets a closure to receive incoming received messages for a session.

func setIncomingMessageHandler((XPCDictionary) -> XPCDictionary?)

Sets a closure to receive incoming dictionary messages for a session.

func cancel(reason: String)

Cancels a session, discarding any unsent messages.

func setCancellationHandler((XPCRichError) -> Void)

Sets a closure the session calls when it’s canceled.

### Sending messages

func send&lt;Message>(Message) throws

Sends an encodable message over the session to the destination service.

func send&lt;Message>(Message, replyHandler: (Result&lt;XPCReceivedMessage, XPCRichError>) -> Void) throws

Sends an encodable message over the session to the destination service, using the closure you specify to handle a reply and rich error.

func send&lt;Message, Reply>(Message, replyHandler: (Result&lt;Reply, any Error>) -> Void) throws

Sends an encodable message over the session to the destination service, using the closure you specify to handle a reply.

func send(message: XPCDictionary) throws

Sends a dictionary message over the session to the destination service.

func send(message: XPCDictionary, replyHandler: (Result&lt;XPCDictionary, XPCRichError>) -> Void)

Sends a message asynchronously over the session to the destination service, calling a closure after receiving a reply.

func sendSync&lt;Message>(Message) throws -> XPCReceivedMessage

Sends an encodable message over the session to the destination service, blocking the caller until receiving a reply message.

func sendSync&lt;Message, Reply>(Message) throws -> Reply

Sends an encodable message over the session to the destination service, blocking the caller until receiving an encodable reply message.

func sendSync(message: XPCDictionary) throws -> XPCDictionary

Sends a dictionary message over the session to the destination service, blocking the caller until receiving a reply.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible

## See Also

### Interprocess communication

Creating XPC services

Configure a listener, establish a client session, and exchange messages between processes.

class XPCListener

A type that performs tasks for clients across process boundaries.

struct XPCReceivedMessage

A type that represents a message sent between a session and a listener.

typealias xpc_listener_t

A C type that performs tasks for clients across process boundaries.

typealias xpc_session_t

A C type that sends messages to a server process.

