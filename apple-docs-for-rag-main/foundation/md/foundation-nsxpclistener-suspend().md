

- Foundation
- NSXPCListener
-  suspend() 

Instance Method

# suspend()

Suspends the listener.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func suspend()
```

## Discussion

As you cannot invalidate a suspended listener, every call to suspend() that you make must be balanced by a call to resume().

## See Also

### Managing connection state

func activate()

Activates the listener.

func resume()

Starts processing of incoming requests.

func invalidate()

Invalidates the listener.

