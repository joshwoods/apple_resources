

- Core Motion
- CMHeadphoneActivityManager
-  startActivityUpdates(to:withHandler:) 

Instance Method

# startActivityUpdates(to:withHandler:)

Starts headphone activity updates, providing data to the given handler through the given queue.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
func startActivityUpdates(
    to queue: OperationQueue,
    withHandler handler: @escaping CMHeadphoneActivityManager.ActivityHandler
)
```

## See Also

### Starting and Stopping Updates

func stopActivityUpdates()

Stops headphone activity updates.

func startStatusUpdates(to: OperationQueue, withHandler: CMHeadphoneActivityManager.StatusHandler)

Starts headphone status updates, providing data to the given handler through the given queue.

func stopStatusUpdates()

Stops headphone status updates.

