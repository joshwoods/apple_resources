

- Core Motion
- CMMotionManager
-  accelerometerData 

Instance Property

# accelerometerData

The latest sample of accelerometer data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var accelerometerData: CMAccelerometerData? { get }
```

## Mentioned in 

Getting raw accelerometer events

## Discussion

If no accelerometer data is available, the value of this property is `nil`. An app that is receiving accelerometer data after calling startAccelerometerUpdates() periodically checks the value of this property and processes the acceleration data.

## See Also

### Managing Accelerometer Updates

var accelerometerUpdateInterval: TimeInterval

The interval, in seconds, for providing accelerometer updates to the block handler.

func startAccelerometerUpdates(to: OperationQueue, withHandler: CMAccelerometerHandler)

Starts accelerometer updates on an operation queue and with a specified handler.

func startAccelerometerUpdates()

Starts accelerometer updates without a handler.

func stopAccelerometerUpdates()

Stops accelerometer updates.

typealias CMAccelerometerHandler

The type of block callback for handling accelerometer data.

