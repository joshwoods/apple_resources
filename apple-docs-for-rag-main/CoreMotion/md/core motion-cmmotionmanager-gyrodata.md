

- Core Motion
- CMMotionManager
-  gyroData 

Instance Property

# gyroData

The latest sample of gyroscope data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var gyroData: CMGyroData? { get }
```

## Mentioned in 

Getting raw gyroscope events

## Discussion

If no gyroscope data is available, the value of this property is `nil`. An app that is receiving gyroscope data after calling startGyroUpdates() periodically checks the value of this property and processes the gyroscope data.

## See Also

### Managing Gyroscope Updates

var gyroUpdateInterval: TimeInterval

The interval, in seconds, for providing gyroscope updates to the block handler.

func startGyroUpdates(to: OperationQueue, withHandler: CMGyroHandler)

Starts gyroscope updates on an operation queue and with a specified handler.

func startGyroUpdates()

Starts gyroscope updates without a handler.

func stopGyroUpdates()

Stops gyroscope updates.

typealias CMGyroHandler

The type of block callback for handling gyroscope data.

