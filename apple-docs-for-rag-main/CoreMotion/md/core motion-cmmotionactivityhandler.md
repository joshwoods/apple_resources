

- Core Motion
-  CMMotionActivityHandler 

Type Alias

# CMMotionActivityHandler

A block that reports the current motion associated with the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
typealias CMMotionActivityHandler = (CMMotionActivity?) -> Void
```

## Discussion

This block takes the following parameter:

`activity`  
The motion activity object that defines the current type of motion for the device.

## See Also

### Starting and Stopping Activity Updates

func startActivityUpdates(to: OperationQueue, withHandler: CMMotionActivityHandler)

Starts the delivery of current motion data updates to your app.

func stopActivityUpdates()

Stops the delivery of motion updates to your app

