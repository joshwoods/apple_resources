

- Foundation
-  NSXPCListenerDelegate 

Protocol

# NSXPCListenerDelegate

The protocol that delegates to the XPC listener use to accept or reject new connections.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSXPCListenerDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func listener(NSXPCListener, shouldAcceptNewConnection: NSXPCConnection) -> Bool

Accepts or rejects a new connection to the listener.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### XPC Services

class NSXPCListener

A listener that waits for new incoming connections, configures them, and accepts or rejects them.

class NSXPCListenerEndpoint

An object that names a specific XPC listener.

