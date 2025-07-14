

- Core Motion
- CMMotionManager
-  startGyroUpdates(to:withHandler:) 

Instance Method

# startGyroUpdates(to:withHandler:)

Starts gyroscope updates on an operation queue and with a specified handler.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
func startGyroUpdates(
    to queue: OperationQueue,
    withHandler handler: @escaping CMGyroHandler
)
```

## Parameters 

`queue`  

An operation queue provided by the caller. Because the processed events might arrive at a high rate, using the main operation queue is not recommended.

`handler`  

A block that is invoked with each update to handle new gyroscope data. The block must conform to the CMGyroHandler type.

## Mentioned in 

Getting raw gyroscope events

## Discussion

You must call stopGyroUpdates() when you no longer want your app to process gyroscope updates.

## See Also

### Managing Gyroscope Updates

var gyroUpdateInterval: TimeInterval

The interval, in seconds, for providing gyroscope updates to the block handler.

func startGyroUpdates()

Starts gyroscope updates without a handler.

func stopGyroUpdates()

Stops gyroscope updates.

var gyroData: CMGyroData?

The latest sample of gyroscope data.

typealias CMGyroHandler

The type of block callback for handling gyroscope data.

