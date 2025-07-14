

- Core Motion
- CMMotionManager
-  startAccelerometerUpdates(to:withHandler:) 

Instance Method

# startAccelerometerUpdates(to:withHandler:)

Starts accelerometer updates on an operation queue and with a specified handler.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
func startAccelerometerUpdates(
    to queue: OperationQueue,
    withHandler handler: @escaping CMAccelerometerHandler
)
```

## Parameters 

`queue`  

An operation queue provided by the caller. Because the processed events might arrive at a high rate, using the main operation queue is not recommended.

`handler`  

A block that is invoked with each update to handle new accelerometer data. The block must conform to the CMAccelerometerHandler type.

## Mentioned in 

Getting raw accelerometer events

## Discussion

You must call stopAccelerometerUpdates() when you no longer want your app to process accelerometer updates.

## See Also

### Managing Accelerometer Updates

var accelerometerUpdateInterval: TimeInterval

The interval, in seconds, for providing accelerometer updates to the block handler.

func startAccelerometerUpdates()

Starts accelerometer updates without a handler.

func stopAccelerometerUpdates()

Stops accelerometer updates.

var accelerometerData: CMAccelerometerData?

The latest sample of accelerometer data.

typealias CMAccelerometerHandler

The type of block callback for handling accelerometer data.

