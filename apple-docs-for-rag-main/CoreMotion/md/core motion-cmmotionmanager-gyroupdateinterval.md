

- Core Motion
- CMMotionManager
-  gyroUpdateInterval 

Instance Property

# gyroUpdateInterval

The interval, in seconds, for providing gyroscope updates to the block handler.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var gyroUpdateInterval: TimeInterval { get set }
```

## Mentioned in 

Getting raw gyroscope events

## Discussion

The system supplies gyroscope (that is, rotation rate) updates to the block handler specified in startGyroUpdates(to:withHandler:) at regular intervals determined by the value of this property. The interval units are in seconds. The value of this property is capped to minimum and maximum values; the maximum value is determined by the maximum frequency supported by the hardware. If your app is sensitive to the intervals of gyroscope data, it should always check the timestamps of the delivered CMGyroData instances to determine the true update interval.

## See Also

### Managing Gyroscope Updates

func startGyroUpdates(to: OperationQueue, withHandler: CMGyroHandler)

Starts gyroscope updates on an operation queue and with a specified handler.

func startGyroUpdates()

Starts gyroscope updates without a handler.

func stopGyroUpdates()

Stops gyroscope updates.

var gyroData: CMGyroData?

The latest sample of gyroscope data.

typealias CMGyroHandler

The type of block callback for handling gyroscope data.

