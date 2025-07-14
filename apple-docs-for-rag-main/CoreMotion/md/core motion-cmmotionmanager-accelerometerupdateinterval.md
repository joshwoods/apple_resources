

- Core Motion
- CMMotionManager
-  accelerometerUpdateInterval 

Instance Property

# accelerometerUpdateInterval

The interval, in seconds, for providing accelerometer updates to the block handler.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var accelerometerUpdateInterval: TimeInterval { get set }
```

## Mentioned in 

Getting raw accelerometer events

## Discussion

The system supplies accelerometer updates to the block handler specified in startAccelerometerUpdates(to:withHandler:) at regular intervals determined by the value of this property. The interval units are in seconds. The value of this property is capped to minimum and maximum values; the maximum value is determined by the maximum frequency supported by the hardware. If your app is sensitive to the intervals of acceleration data, it should always check the timestamps of the delivered CMAccelerometerData instances to determine the true update interval.

## See Also

### Related Documentation

Event Handling Guide for UIKit Apps

### Managing Accelerometer Updates

func startAccelerometerUpdates(to: OperationQueue, withHandler: CMAccelerometerHandler)

Starts accelerometer updates on an operation queue and with a specified handler.

func startAccelerometerUpdates()

Starts accelerometer updates without a handler.

func stopAccelerometerUpdates()

Stops accelerometer updates.

var accelerometerData: CMAccelerometerData?

The latest sample of accelerometer data.

typealias CMAccelerometerHandler

The type of block callback for handling accelerometer data.

