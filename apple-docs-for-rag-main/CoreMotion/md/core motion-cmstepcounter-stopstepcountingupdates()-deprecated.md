

- Core Motion
- CMStepCounter
-  stopStepCountingUpdates() Deprecated

Instance Method

# stopStepCountingUpdates()

Stops the delivery of step-counting updates to your app.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func stopStepCountingUpdates()
```

Deprecated

Use CMPedometer instead

## Discussion

Call this method to stop the delivery of updates that you started by calling the startStepCountingUpdates(to:updateOn:withHandler:) method. This method does not stop queries started using the queryStepCountStarting(from:to:to:withHandler:) method.

## See Also

### Starting and Stopping Step Counting Updates

func startStepCountingUpdates(to: OperationQueue, updateOn: Int, withHandler: CMStepUpdateHandler)

Starts the delivery of current step-counting data to your app.

Deprecated

typealias CMStepUpdateHandler

A block that reports the number of steps recorded since updates began.

