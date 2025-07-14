

- Core Motion
- CMMotionManager
-  stopAccelerometerUpdates() 

Instance Method

# stopAccelerometerUpdates()

Stops accelerometer updates.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
func stopAccelerometerUpdates()
```

## See Also

### Managing Accelerometer Updates

var accelerometerUpdateInterval: TimeInterval

The interval, in seconds, for providing accelerometer updates to the block handler.

func startAccelerometerUpdates(to: OperationQueue, withHandler: CMAccelerometerHandler)

Starts accelerometer updates on an operation queue and with a specified handler.

func startAccelerometerUpdates()

Starts accelerometer updates without a handler.

var accelerometerData: CMAccelerometerData?

The latest sample of accelerometer data.

typealias CMAccelerometerHandler

The type of block callback for handling accelerometer data.

