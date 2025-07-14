

- Foundation
-  NSXPCListener 

Class

# NSXPCListener

A listener that waits for new incoming connections, configures them, and accepts or rejects them.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSXPCListener
```

## Overview

Each XPC service, launchd agent, or launchd daemon typically has at least one NSXPCListener object that listens for connections to a specified service name. Each listener must have a delegate that conforms to the NSXPCListenerDelegate protocol. When the listener receives a new connection request, it creates a new NSXPCConnection object, then asks the delegate to inspect, configure, and resume the connection object by calling the delegate’s listener(_:shouldAcceptNewConnection:) method.

## Topics

### Creating a listener

init(machServiceName: String)

Initializes a listener in a LaunchAgent or LaunchDaemon which has a name advertised in a `launchd.plist` file.

### Using standard listeners

class func service() -> NSXPCListener

Returns the singleton listener used to listen for incoming connections in an XPC service.

class func anonymous() -> NSXPCListener

Returns a new anonymous listener connection.

### Working with a delegate

var delegate: (any NSXPCListenerDelegate)?

The delegate for the listener.

### Providing access to clients

var endpoint: NSXPCListenerEndpoint

Returns an endpoint object that may be sent over an existing connection.

### Managing connection state

func activate()

Activates the listener.

func resume()

Starts processing of incoming requests.

func invalidate()

Invalidates the listener.

func suspend()

Suspends the listener.

### Working with code-signing

func setConnectionCodeSigningRequirement(String)

Sets the code signing requirement for connections to this listener.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### XPC Services

protocol NSXPCListenerDelegate

The protocol that delegates to the XPC listener use to accept or reject new connections.

class NSXPCListenerEndpoint

An object that names a specific XPC listener.

