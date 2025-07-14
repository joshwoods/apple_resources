

- XPC
- XPCListener
- XPCListener.IncomingSessionRequest
-  accept(\_:) 

Instance Method

# accept(\_:)

Accepts an incoming session request from a client, delegating incoming received messages to a separate object.

Mac Catalyst 17.0+macOS 14.0+

``` source
func accept(_ inactiveSessionHandler: (XPCSession) -> Handler) -> XPCListener.IncomingSessionRequest.Decision where Handler : XPCPeerHandler, Handler.Input == XPCReceivedMessage, Handler.Output == any Encodable
```

## Parameters 

`inactiveSessionHandler`  

A closure that receives an inactive incoming session and returns an object to handle messages in the session.

## Return Value

A decision that indicates whether the listener accepts or rejects the incoming session.

## See Also

### Responding to client sessions requests

func accept&lt;Handler>((XPCSession) -> Handler) -> XPCListener.IncomingSessionRequest.Decision

Accepts an incoming session request from a client, delegating incoming encodable messages to a separate object.

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

func accept(incomingMessageHandler: (XPCDictionary) -> XPCDictionary?, cancellationHandler: ((XPCRichError) -> Void)?) -> (XPCListener.IncomingSessionRequest.Decision, XPCSession)

Accepts an incoming session request from a client using a closure to handle dictionary messages, and returns the inactive session.

func reject(reason: String) -> XPCListener.IncomingSessionRequest.Decision

Rejects an incoming client session request.

struct Decision

An opaque type that indicates whether a listener accepts or rejects an incoming session request.

