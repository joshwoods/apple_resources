

- AccessorySetupKit
- ASAccessorySession
-  invalidate() 

Instance Method

# invalidate()

Invalidate the session by stopping any operations.

iOS 18.0+iPadOS 18.0+

``` source
func invalidate()
```

## Discussion

This call breaks any retain cycles. The session is unusable after calling `invalidate`.

## See Also

### Managing the session life cycle

func activate(on: dispatch_queue_t, eventHandler: (ASAccessoryEvent) -> Void)

Activate the session and start delivering events to an event handler.

