

- Foundation
- NSXPCConnection
-  invalidationHandler 

Instance Property

# invalidationHandler

An invalidation handler that is called if the connection can not be formed or the connection has terminated and may not be re-established.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var invalidationHandler: (() -> Void)? { get set }
```

## Discussion

This handler is invoked on the same queue as reply messages and other handlers, and is always executed last (after the interruption handler, if required). You may not send messages over the connection from within an invalidation handler block.

## See Also

### Managing connection state

func activate()

Activates the connection.

func resume()

Starts or resumes handling of messages on a connection.

func invalidate()

Invalidates the connection.

func suspend()

Suspends the connection.

var interruptionHandler: (() -> Void)?

An interruption handler that is called if the remote process exits or crashes.

class func current() -> NSXPCConnection?

Returns the current connection, in the context of a call to a method on your exported object.

func scheduleSendBarrierBlock(() -> Void)

Add a barrier block to execute on the connection.

