

- Foundation
- NSXPCListener
-  activate() 

Instance Method

# activate()

Activates the listener.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func activate()
```

## Discussion

Connections start in an inactive state. You must call activate() on a connection before it can send or receive any messages.

Calling activate() on an active connection has no effect.

For backward compatibility reasons, calling resume() on an inactive and otherwise not suspended NSXPCListener has the same effect as calling activate(). For new code, prefer activate().

## See Also

### Managing connection state

func resume()

Starts processing of incoming requests.

func invalidate()

Invalidates the listener.

func suspend()

Suspends the listener.

