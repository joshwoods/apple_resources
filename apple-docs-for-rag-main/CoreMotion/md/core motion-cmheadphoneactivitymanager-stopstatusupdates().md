

- Core Motion
- CMHeadphoneActivityManager
-  stopStatusUpdates() 

Instance Method

# stopStatusUpdates()

Stops headphone status updates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
func stopStatusUpdates()
```

## See Also

### Starting and Stopping Updates

func startActivityUpdates(to: OperationQueue, withHandler: CMHeadphoneActivityManager.ActivityHandler)

Starts headphone activity updates, providing data to the given handler through the given queue.

func stopActivityUpdates()

Stops headphone activity updates.

func startStatusUpdates(to: OperationQueue, withHandler: CMHeadphoneActivityManager.StatusHandler)

Starts headphone status updates, providing data to the given handler through the given queue.

