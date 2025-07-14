

- Foundation
- NSXPCListener
-  resume() 

Instance Method

# resume()

Starts processing of incoming requests.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func resume()
```

## Discussion

All listeners start suspended and must be resumed before they begin processing incoming requests.

If called on the service() object, this method never returns. Therefore, you should call it as the last step inside the XPC service’s `main` function after setting up any desired initial state and configuring the listener itself.

If called on any other NSXPCListener, the connection is resumed, and the method returns immediately.

## See Also

### Managing connection state

func activate()

Activates the listener.

func invalidate()

Invalidates the listener.

func suspend()

Suspends the listener.

