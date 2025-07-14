

- XPC
-  XPCListener 

Class

# XPCListener

A type that performs tasks for clients across process boundaries.

Mac Catalyst 17.0+macOS 14.0+

``` source
class XPCListener
```

## Mentioned in 

Creating XPC services

## Overview

To implement an XPC service, create a listener and respond to incoming session requests.

## Topics

### Creating a listener

init(service: String, targetQueue: DispatchQueue?, options: XPCListener.InitializationOptions, incomingSessionHandler: (XPCListener.IncomingSessionRequest) -> XPCListener.IncomingSessionRequest.Decision) throws

Creates the server side of an XPC service using the specified service name.

struct InitializationOptions

Options that control the listener’s configuration, such as if it’s inactive at creation.

class IncomingSessionRequest

A session request from a client that you accept or reject.

### Managing the life cycle

func activate() throws

Activates an inactive listener.

func cancel()

Cancels a listener.

### Handling incoming messages

protocol XPCPeerHandler

A type that handles incoming messages from a client and session cancellation.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible

## See Also

### Interprocess communication

Creating XPC services

Configure a listener, establish a client session, and exchange messages between processes.

class XPCSession

A type that sends messages to a server process.

struct XPCReceivedMessage

A type that represents a message sent between a session and a listener.

typealias xpc_listener_t

A C type that performs tasks for clients across process boundaries.

typealias xpc_session_t

A C type that sends messages to a server process.

