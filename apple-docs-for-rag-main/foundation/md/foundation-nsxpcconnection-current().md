

- Foundation
- NSXPCConnection
-  current() 

Type Method

# current()

Returns the current connection, in the context of a call to a method on your exported object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func current() -> NSXPCConnection?
```

## Return Value

An NSXPCConnection object, representing a connection to another process.

## Discussion

Use this method to determine what process invoked the current call.

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

var invalidationHandler: (() -> Void)?

An invalidation handler that is called if the connection can not be formed or the connection has terminated and may not be re-established.

func scheduleSendBarrierBlock(() -> Void)

Add a barrier block to execute on the connection.

