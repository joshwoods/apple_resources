

- XPC
- XPCSession
-  activate() 

Instance Method

# activate()

Activates a session so you can send messages.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func activate() throws
```

## Discussion

Important

Don’t call activate() on a session that’s already active.

If you create an inactive session using the inactive initialization option, you must activate the session before deinitialization. Deinitializing an inactive session causes the process to crash.

If activation fails, this method automatically cancels the session and throws a XPCRichError that describes the reason activation failed.

## See Also

### Managing the life cycle

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

