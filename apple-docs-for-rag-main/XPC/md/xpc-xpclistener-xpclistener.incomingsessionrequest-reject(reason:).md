

- XPC
- XPCListener
- XPCListener.IncomingSessionRequest
-  reject(reason:) 

Instance Method

# reject(reason:)

Rejects an incoming client session request.

Mac Catalyst 17.0+macOS 14.0+

``` source
func reject(reason: String) -> XPCListener.IncomingSessionRequest.Decision
```

## Parameters 

`reason`  

A description of why the listener rejected the request.

## Return Value

A decision that indicates that the request was canceled.

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

func accept(incomingMessageHandler: (XPCDictionary) -> XPCDictionary?, cancellationHandler: ((XPCRichError) -> Void)?) -> (XPCListener.IncomingSessionRequest.Decision, XPCSession)

Accepts an incoming session request from a client using a closure to handle dictionary messages, and returns the inactive session.

struct Decision

An opaque type that indicates whether a listener accepts or rejects an incoming session request.

