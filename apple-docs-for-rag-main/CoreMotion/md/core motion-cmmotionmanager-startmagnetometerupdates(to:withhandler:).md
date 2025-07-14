

- Core Motion
- CMMotionManager
-  startMagnetometerUpdates(to:withHandler:) 

Instance Method

# startMagnetometerUpdates(to:withHandler:)

Starts magnetometer updates on an operation queue and with a specified handler.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func startMagnetometerUpdates(
    to queue: OperationQueue,
    withHandler handler: @escaping CMMagnetometerHandler
)
```

## Parameters 

`queue`  

An operation queue provided by the caller. Because the processed events might arrive at a high rate, using the main operation queue is not recommended.

`handler`  

A block that is invoked with each update to handle new magnetometer data. The block must conform to the CMMagnetometerHandler type.

## Discussion

You must call stopMagnetometerUpdates() when you no longer want your app to process magnetometer updates.

## See Also

### Managing Magnetometer Updates

var magnetometerUpdateInterval: TimeInterval

The interval, in seconds, at which the system delivers magnetometer data to the block handler.

func startMagnetometerUpdates()

Starts magnetometer updates without a block handler.

func stopMagnetometerUpdates()

Stops magnetometer updates.

var magnetometerData: CMMagnetometerData?

The latest sample of magnetometer data.

typealias CMMagnetometerHandler

The type of block callback for handling magnetometer data.

