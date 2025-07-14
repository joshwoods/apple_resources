

- XPC
- XPCSession
-  cancel(reason:) 

Instance Method

# cancel(reason:)

Cancels a session, discarding any unsent messages.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func cancel(reason: String)
```

## Parameters 

`reason`  

A description that explains why cancellation occured.

## Discussion

When you cancel a session, it discards any unsent messages and invalidates its connection. If there are messages awaiting replies, the session calls the reply handlers with an appropriate XPCRichError.

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

func setCancellationHandler((XPCRichError) -> Void)

Sets a closure the session calls when it’s canceled.

