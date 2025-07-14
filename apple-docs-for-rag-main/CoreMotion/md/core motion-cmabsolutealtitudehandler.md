

- Core Motion
-  CMAbsoluteAltitudeHandler 

Type Alias

# CMAbsoluteAltitudeHandler

A block for receiving absolute altitude data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias CMAbsoluteAltitudeHandler = (CMAbsoluteAltitudeData?, (any Error)?) -> Void
```

## Parameters 

`altitudeData`  

The current altitude for the device. If there’s an error generating the data, this parameter is `nil`.

`error`  

The error object. Returns `nil` if the altimeter successfully delivers the altitude data. When an error occurs, you can use the information in the provided object to recover the data or to alert the user.

## Discussion

You pass a block of this type to the altimeter object’s startAbsoluteAltitudeUpdates(to:withHandler:) method when starting the delivery of altitude data.

Note

Absolute altitude is only available on iPhone 12 and later and Apple Watch 6 or SE and later.

## See Also

### Starting and Stopping Altitude Updates

func startAbsoluteAltitudeUpdates(to: OperationQueue, withHandler: CMAbsoluteAltitudeHandler)

Starts the delivery of absolute altitude data to the specified handler.

func stopAbsoluteAltitudeUpdates()

Stops the delivery of absolute altitude data for this altimeter object.

func startRelativeAltitudeUpdates(to: OperationQueue, withHandler: CMAltitudeHandler)

Starts the delivery of relative altitude data to the specified handler.

func stopRelativeAltitudeUpdates()

Stops the delivery of relative altitude data for the altimeter object.

typealias CMAltitudeHandler

A block for receiving relative altitude data.

