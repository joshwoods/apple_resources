

- Core Motion
- CMMotionActivityManager
-  stopActivityUpdates() 

Instance Method

# stopActivityUpdates()

Stops the delivery of motion updates to your app

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func stopActivityUpdates()
```

## Discussion

Call this method to stop the delivery of updates that you started by calling the startActivityUpdates(to:withHandler:) method. This method does not stop queries started using the queryActivityStarting(from:to:to:withHandler:) method.

## See Also

### Starting and Stopping Activity Updates

func startActivityUpdates(to: OperationQueue, withHandler: CMMotionActivityHandler)

Starts the delivery of current motion data updates to your app.

typealias CMMotionActivityHandler

A block that reports the current motion associated with the device.

