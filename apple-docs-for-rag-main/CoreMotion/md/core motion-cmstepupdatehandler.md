

- Core Motion
-  CMStepUpdateHandler 

Type Alias

# CMStepUpdateHandler

A block that reports the number of steps recorded since updates began.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
typealias CMStepUpdateHandler = (Int, Date, (any Error)?) -> Void
```

## Discussion

This block takes the following parameters:

`numberOfSteps`  
The total number of steps since the startStepCountingUpdates(to:updateOn:withHandler:) method was called.

`timestamp`  
The time at which the current step count was reported.

`error`  
An error object indicating that there was a problem gathering the data or `nil` if the number of steps was determined correctly.

## See Also

### Starting and Stopping Step Counting Updates

func startStepCountingUpdates(to: OperationQueue, updateOn: Int, withHandler: CMStepUpdateHandler)

Starts the delivery of current step-counting data to your app.

Deprecated

func stopStepCountingUpdates()

Stops the delivery of step-counting updates to your app.

Deprecated

