

- Core Motion
- CMAltimeter
-  startRelativeAltitudeUpdates(to:withHandler:) 

Instance Method

# startRelativeAltitudeUpdates(to:withHandler:)

Starts the delivery of relative altitude data to the specified handler.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func startRelativeAltitudeUpdates(
    to queue: OperationQueue,
    withHandler handler: @escaping CMAltitudeHandler
)
```

## Parameters 

`queue`  

The operation queue on which to execute your handler block. The altimeter object stores a strong reference to this object. This parameter must not be `nil`.

`handler`  

The handler block to execute when new altitude data is available. This parameter must not be `nil`. For information about the format of this block, see CMAltitudeHandler.

## Discussion

Call this method to initiate the delivery of events. The altimeter object stores a strong reference to the specified queue and makes a copy of your block. If you call the method a second time, the altimeter object releases its references to the previous queue and handler before storing references to the new ones. Only the last installed handler receives events. When you no longer need the altitude data, or when an error occurs, call the stopRelativeAltitudeUpdates() method to stop the delivery of events.

If altitude data isn’t available on the current device, this method does nothing.

## See Also

### Starting and Stopping Altitude Updates

func startAbsoluteAltitudeUpdates(to: OperationQueue, withHandler: CMAbsoluteAltitudeHandler)

Starts the delivery of absolute altitude data to the specified handler.

func stopAbsoluteAltitudeUpdates()

Stops the delivery of absolute altitude data for this altimeter object.

typealias CMAbsoluteAltitudeHandler

A block for receiving absolute altitude data.

func stopRelativeAltitudeUpdates()

Stops the delivery of relative altitude data for the altimeter object.

typealias CMAltitudeHandler

A block for receiving relative altitude data.

