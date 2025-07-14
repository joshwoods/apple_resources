

- Foundation
- NSXPCConnection
-  resume() 

Instance Method

# resume()

Starts or resumes handling of messages on a connection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func resume()
```

## Discussion

All connections start suspended. You must resume them before they start processing received messages or sending messages through the remoteObjectProxy() object.

## See Also

### Managing connection state

func activate()

Activates the connection.

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

