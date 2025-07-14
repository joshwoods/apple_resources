

- XPC
- XPCSession
-  setCancellationHandler(\_:) 

Instance Method

# setCancellationHandler(\_:)

Sets a closure the session calls when it’s canceled.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func setCancellationHandler(_ cancellationHandler: @escaping (XPCRichError) -> Void)
```

## Parameters 

`cancellationHandler`  

A closure that receives an error indicating why the session was canceled.

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

func setIncomingMessageHandler((XPCDictionary) -> XPCDictionary?)

Sets a closure to receive incoming dictionary messages for a session.

func cancel(reason: String)

Cancels a session, discarding any unsent messages.

