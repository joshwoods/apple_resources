

- Exposure Notification
- ENManager
-  invalidate() 

Instance Method

# invalidate()

Stops any outstanding operations and invalidates the manager.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
func invalidate()
```

## Discussion

Important

This method is available in iOS 12.5, and in iOS 13.5 and later.

Once you call this method, the object can no longer be used. To start using ENManager again, create and activate a new instance of the class.

## Topics

### Completion Handlers

var invalidationHandler: (() -> Void)?

The handler that the framework invokes when invalidation completes.

