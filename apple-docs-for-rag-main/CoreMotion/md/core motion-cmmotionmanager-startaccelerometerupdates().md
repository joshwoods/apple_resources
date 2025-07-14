

- Core Motion
- CMMotionManager
-  startAccelerometerUpdates() 

Instance Method

# startAccelerometerUpdates()

Starts accelerometer updates without a handler.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
func startAccelerometerUpdates()
```

## Mentioned in 

Getting raw accelerometer events

## Discussion

You can get the latest accelerometer data through the accelerometerData property. You must call stopAccelerometerUpdates() when you no longer want your app to process accelerometer updates.

## See Also

### Managing Accelerometer Updates

var accelerometerUpdateInterval: TimeInterval

The interval, in seconds, for providing accelerometer updates to the block handler.

func startAccelerometerUpdates(to: OperationQueue, withHandler: CMAccelerometerHandler)

Starts accelerometer updates on an operation queue and with a specified handler.

func stopAccelerometerUpdates()

Stops accelerometer updates.

var accelerometerData: CMAccelerometerData?

The latest sample of accelerometer data.

typealias CMAccelerometerHandler

The type of block callback for handling accelerometer data.

