

- Core Motion
- CMAltimeter
-  startAbsoluteAltitudeUpdates(to:withHandler:) 

Instance Method

# startAbsoluteAltitudeUpdates(to:withHandler:)

Starts the delivery of absolute altitude data to the specified handler.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+watchOS 8.0+

``` source
func startAbsoluteAltitudeUpdates(
    to queue: OperationQueue,
    withHandler handler: @escaping CMAbsoluteAltitudeHandler
)
```

## Parameters 

`queue`  

The operation queue on which to execute your handler block. The altimeter object stores a strong reference to this object. This parameter must not be `nil`.

`handler`  

The handler block to execute when new altitude data is available. This parameter must not be `nil`. For information about the format of this block, see CMAbsoluteAltitudeHandler.

## Discussion

Call isAbsoluteAltitudeAvailable() to verify that the current device supports absolute altitude updates before calling the `startAbsoluteAltitudeUpdates(to:withHandler:)` method.

Note

Absolute altitude is only available on iPhone 12 and later and Apple Watch 6 or SE and later.

## See Also

### Starting and Stopping Altitude Updates

func stopAbsoluteAltitudeUpdates()

Stops the delivery of absolute altitude data for this altimeter object.

typealias CMAbsoluteAltitudeHandler

A block for receiving absolute altitude data.

func startRelativeAltitudeUpdates(to: OperationQueue, withHandler: CMAltitudeHandler)

Starts the delivery of relative altitude data to the specified handler.

func stopRelativeAltitudeUpdates()

Stops the delivery of relative altitude data for the altimeter object.

typealias CMAltitudeHandler

A block for receiving relative altitude data.

