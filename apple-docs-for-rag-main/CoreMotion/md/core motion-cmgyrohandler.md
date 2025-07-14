

- Core Motion
-  CMGyroHandler 

Type Alias

# CMGyroHandler

The type of block callback for handling gyroscope data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
typealias CMGyroHandler = (CMGyroData?, (any Error)?) -> Void
```

## Discussion

Blocks of type `CMGyroHandler` are called when there is gyroscope data to process. You pass the block into startGyroUpdates(to:withHandler:) as the second argument. Blocks of this type return no value but take two arguments:

`gyroData`  
An object that encapsulates a CMRotationRate structure with fields holding rotation-rate values for the three axes of movement.

`error`  
An error object representing an error encountered in providing gyroscope data. If an error occurs, you should stop gyroscope updates and inform the user of the problem. If there is no error, this argument is `nil`. Core Motion errors are of the CMErrorDomain domain and the CMError type.

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

var gyroData: CMGyroData?

The latest sample of gyroscope data.

