

- Foundation
- NSXPCListener
-  invalidate() 

Instance Method

# invalidate()

Invalidates the listener.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func invalidate()
```

## Discussion

After calling this method, no more connections are created. Once a listener is invalidated it may not be resumed or suspended.

## See Also

### Managing connection state

func activate()

Activates the listener.

func resume()

Starts processing of incoming requests.

func suspend()

Suspends the listener.

