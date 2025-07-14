

- Core Motion
-  CMAltitudeHandler 

Type Alias

# CMAltitudeHandler

A block for receiving relative altitude data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
typealias CMAltitudeHandler = (CMAltitudeData?, (any Error)?) -> Void
```

## Parameters 

`altitudeData`  

The relative change in altitude data. If there’s an error generating the data, this parameter is `nil`.

`error`  

The error object. Returns `nil` if the altimeter successfully delivers the altitude data. When an error occurs, you can use the information in the provided object to recover the data or to alert the user.

## Discussion

You pass a block of this type to the altimeter object’s startRelativeAltitudeUpdates(to:withHandler:) method when starting the delivery of altitude data.

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

func stopRelativeAltitudeUpdates()

Stops the delivery of relative altitude data for the altimeter object.

