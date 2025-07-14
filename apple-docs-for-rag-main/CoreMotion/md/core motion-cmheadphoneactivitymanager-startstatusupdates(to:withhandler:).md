

- Core Motion
- CMHeadphoneActivityManager
-  startStatusUpdates(to:withHandler:) 

Instance Method

# startStatusUpdates(to:withHandler:)

Starts headphone status updates, providing data to the given handler through the given queue.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
func startStatusUpdates(
    to queue: OperationQueue,
    withHandler handler: @escaping CMHeadphoneActivityManager.StatusHandler
)
```

## Discussion

If a compatible set of headphones is already connected before you call this method, the handler is called with a status update of CMHeadphoneActivityManager.Status.connected for the connected headphones.

## See Also

### Starting and Stopping Updates

func startActivityUpdates(to: OperationQueue, withHandler: CMHeadphoneActivityManager.ActivityHandler)

Starts headphone activity updates, providing data to the given handler through the given queue.

func stopActivityUpdates()

Stops headphone activity updates.

func stopStatusUpdates()

Stops headphone status updates.

