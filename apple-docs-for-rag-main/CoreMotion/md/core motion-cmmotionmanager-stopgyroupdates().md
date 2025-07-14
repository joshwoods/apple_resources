

- Core Motion
- CMMotionManager
-  stopGyroUpdates() 

Instance Method

# stopGyroUpdates()

Stops gyroscope updates.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
func stopGyroUpdates()
```

## See Also

### Managing Gyroscope Updates

var gyroUpdateInterval: TimeInterval

The interval, in seconds, for providing gyroscope updates to the block handler.

func startGyroUpdates(to: OperationQueue, withHandler: CMGyroHandler)

Starts gyroscope updates on an operation queue and with a specified handler.

func startGyroUpdates()

Starts gyroscope updates without a handler.

var gyroData: CMGyroData?

The latest sample of gyroscope data.

typealias CMGyroHandler

The type of block callback for handling gyroscope data.

