

- Core Motion
-  CMAccelerometerHandler 

Type Alias

# CMAccelerometerHandler

The type of block callback for handling accelerometer data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
typealias CMAccelerometerHandler = (CMAccelerometerData?, (any Error)?) -> Void
```

## Discussion

Blocks of type `CMAccelerometerHandler` are called when there is accelerometer data to process. You pass the block into startAccelerometerUpdates(to:withHandler:) as the second argument. Blocks of this type return no value but take two arguments:

`accelerometerData`  
An object that encapsulates a CMAcceleration structure with fields holding acceleration values for the three axes of movement.

`error`  
An error object representing an error encountered in providing accelerometer updates. If an error occurs, you should stop accelerometer updates and inform the user of the problem. If there is no error, this argument is `nil`. Core Motion errors are of the CMErrorDomain domain and the CMError type.

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

var accelerometerData: CMAccelerometerData?

The latest sample of accelerometer data.

