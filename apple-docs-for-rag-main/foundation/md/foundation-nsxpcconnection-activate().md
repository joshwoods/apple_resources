

- Foundation
- NSXPCConnection
-  activate() 

Instance Method

# activate()

Activates the connection.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func activate()
```

## Discussion

Connections start in an inactive state. You must call activate() on a connection before it can send or receive any messages.

Calling activate() on an active connection has no effect.

For backward compatibility reasons, calling resume() on an inactive and otherwise not suspended NSXPCConnection has the same effect as calling activate(). For new code, prefer activate().

## See Also

### Managing connection state

func resume()

Starts or resumes handling of messages on a connection.

func invalidate()

Invalidates the connection.

func suspend()

Suspends the connection.

var interruptionHandler: (() -> Void)?

An interruption handler that is called if the remote process exits or crashes.

var invalidationHandler: (() -> Void)?

An invalidation handler that is called if the connection can not be formed or the connection has terminated and may not be re-established.

class func current() -> NSXPCConnection?

Returns the current connection, in the context of a call to a method on your exported object.

func scheduleSendBarrierBlock(() -> Void)

Add a barrier block to execute on the connection.

