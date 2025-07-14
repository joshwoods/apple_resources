

- Core Motion
- CMAltimeter
-  stopRelativeAltitudeUpdates() 

Instance Method

# stopRelativeAltitudeUpdates()

Stops the delivery of relative altitude data for the altimeter object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func stopRelativeAltitudeUpdates()
```

## Discussion

Calling this method ends the delivery of relative altitude events and releases the references to the operation queue and block that you specified in the startRelativeAltitudeUpdates(to:withHandler:) method. If you haven’t started delivering data, or if you’ve already called stopRelativeAltitudeUpdates(), this method does nothing.

## See Also

### Starting and Stopping Altitude Updates

func startAbsoluteAltitudeUpdates(to: OperationQueue, withHandler: CMAbsoluteAltitudeHandler)

Starts the delivery of absolute altitude data to the specified handler.

func stopAbsoluteAltitudeUpdates()

Stops the delivery of absolute altitude data for this altimeter object.

typealias CMAbsoluteAltitudeHandler

A block for receiving absolute altitude data.

func startRelativeAltitudeUpdates(to: OperationQueue, withHandler: CMAltitudeHandler)

Starts the delivery of relative altitude data to the specified handler.

typealias CMAltitudeHandler

A block for receiving relative altitude data.

