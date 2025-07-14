

- XPC
- XPCSession
-  setIncomingMessageHandler(\_:) 

Instance Method

# setIncomingMessageHandler(\_:)

Sets a closure to receive incoming dictionary messages for a session.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func setIncomingMessageHandler(_ incomingMessageHandler: @escaping (XPCDictionary) -> XPCDictionary?)
```

## Parameters 

`incomingMessageHandler`  

A closure that the session invokes when it receives messages. The closure has a parameter that contains the message from the client, and optionally returns a dictionary reply message to returns to the client. If the closure returns Nil, you can use send(message:) to reply asynchronously after the closure completes.

## Discussion

Important

Only call this method on an inactive session.

## See Also

### Managing the life cycle

func activate() throws

Activates a session so you can send messages.

func setIncomingMessageHandler&lt;Message>((Message) -> (any Encodable)?)

Sets a closure to receive incoming decodable messages for a session.

func setIncomingMessageHandler((XPCReceivedMessage) -> (any Encodable)?)

Sets a closure to receive incoming received messages for a session.

func cancel(reason: String)

Cancels a session, discarding any unsent messages.

func setCancellationHandler((XPCRichError) -> Void)

Sets a closure the session calls when it’s canceled.

