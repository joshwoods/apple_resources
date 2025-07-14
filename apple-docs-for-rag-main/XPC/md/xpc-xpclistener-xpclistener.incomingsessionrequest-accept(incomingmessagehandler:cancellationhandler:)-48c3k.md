

- XPC
- XPCListener
- XPCListener.IncomingSessionRequest
-  accept(incomingMessageHandler:cancellationHandler:) 

Instance Method

# accept(incomingMessageHandler:cancellationHandler:)

Accepts an incoming session request from a client using a closure to handle dictionary messages, and returns the inactive session.

Mac Catalyst 17.0+macOS 14.0+

``` source
func accept(
    incomingMessageHandler: @escaping (XPCDictionary) -> XPCDictionary?,
    cancellationHandler: ((XPCRichError) -> Void)? = nil
) -> (XPCListener.IncomingSessionRequest.Decision, XPCSession)
```

## Parameters 

`incomingMessageHandler`  

A closure that receives incoming messages from a client.

`cancellationHandler`  

An optional closure that the system invokes when it cancels the session.

## Return Value

A tuple that indicates whether the listener accepts or rejects the incoming session, and includes the inactive session.

## Discussion

The difference between this method and accept(incomingMessageHandler:cancellationHandler:) is to allow the listener to configure the session, if needed. If you don’t need to perform any session configuration, use accept(incomingMessageHandler:cancellationHandler:) instead.

## See Also

### Responding to client sessions requests

func accept&lt;Handler>((XPCSession) -> Handler) -> XPCListener.IncomingSessionRequest.Decision

Accepts an incoming session request from a client, delegating incoming encodable messages to a separate object.

func accept&lt;Handler>((XPCSession) -> Handler) -> XPCListener.IncomingSessionRequest.Decision

Accepts an incoming session request from a client, delegating incoming received messages to a separate object.

func accept&lt;Handler>((XPCSession) -> Handler) -> XPCListener.IncomingSessionRequest.Decision

Accepts an incoming session request from a client, delegating incoming dictionary messages to a separate object.

func accept&lt;Message>(incomingMessageHandler: (Message) -> (any Encodable)?, cancellationHandler: ((XPCRichError) -> Void)?) -> XPCListener.IncomingSessionRequest.Decision

Accepts an incoming session request from a client using closures to handle encodable messages or cancellation, and returns the inactive session.

func accept(incomingMessageHandler: (XPCReceivedMessage) -> (any Encodable)?, cancellationHandler: ((XPCRichError) -> Void)?) -> XPCListener.IncomingSessionRequest.Decision

Accepts an incoming session request from a client using closures to handle received messages or cancellation, and returns the inactive session.

func accept(incomingMessageHandler: (XPCDictionary) -> XPCDictionary?, cancellationHandler: ((XPCRichError) -> Void)?) -> XPCListener.IncomingSessionRequest.Decision

Accepts an incoming session request from a client using closures to handle dictionary messages or cancellation, and returns the inactive session.

func accept&lt;Message>(incomingMessageHandler: (Message) -> (any Encodable)?, cancellationHandler: ((XPCRichError) -> Void)?) -> (XPCListener.IncomingSessionRequest.Decision, XPCSession)

Accepts an incoming session request from a client using a closure to handle encodable messages, and returns the inactive session.

func accept(incomingMessageHandler: (XPCReceivedMessage) -> (any Encodable)?, cancellationHandler: ((XPCRichError) -> Void)?) -> (XPCListener.IncomingSessionRequest.Decision, XPCSession)

Accepts an incoming session request from a client using a closure to handle received messages, and returns the inactive session.

func reject(reason: String) -> XPCListener.IncomingSessionRequest.Decision

Rejects an incoming client session request.

struct Decision

An opaque type that indicates whether a listener accepts or rejects an incoming session request.

