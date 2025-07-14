

- XPC
- XPCListener
-  XPCListener.IncomingSessionRequest 

Class

# XPCListener.IncomingSessionRequest

A session request from a client that you accept or reject.

Mac Catalyst 17.0+macOS 14.0+

``` source
class IncomingSessionRequest
```

## Mentioned in 

Creating XPC services

## Overview

When a client initiates a connection to a listener, the system passes the incoming session request to the listener. In response, the listener calls one of the `accept` methods to complete the connection with the client, or it rejects the request.

## Topics

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

func reject(reason: String) -> XPCListener.IncomingSessionRequest.Decision

Rejects an incoming client session request.

struct Decision

An opaque type that indicates whether a listener accepts or rejects an incoming session request.

## See Also

### Creating a listener

init(service: String, targetQueue: DispatchQueue?, options: XPCListener.InitializationOptions, incomingSessionHandler: (XPCListener.IncomingSessionRequest) -> XPCListener.IncomingSessionRequest.Decision) throws

Creates the server side of an XPC service using the specified service name.

struct InitializationOptions

Options that control the listener’s configuration, such as if it’s inactive at creation.

