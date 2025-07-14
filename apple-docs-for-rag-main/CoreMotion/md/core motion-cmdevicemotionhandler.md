

- Core Motion
-  CMDeviceMotionHandler 

Type Alias

# CMDeviceMotionHandler

The type of block callback for handling device-motion data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
typealias CMDeviceMotionHandler = (CMDeviceMotion?, (any Error)?) -> Void
```

## Mentioned in 

Getting processed device-motion data

## Discussion

Blocks of type `CMDeviceMotionHandler` are called when there is device-motion data to process. You pass the block into startDeviceMotionUpdates(to:withHandler:) as the second argument. Blocks of this type return no value but take two arguments:

`motion`  
A CMDeviceMotion object, which encapsulates other objects and a structure representing attitude, rotation rate, gravity, and user acceleration.

`error`  
An error object representing an error encountered in providing device-motion data. If an error occurs, you should stop device-motion data updates and inform the user of the problem. If there is no error, this argument is `nil`. Core Motion errors are of the CMErrorDomain domain and the CMError type.

## See Also

### Managing Device Motion Updates

var showsDeviceMovementDisplay: Bool

Controls whether the device-movement display is shown.

var deviceMotionUpdateInterval: TimeInterval

The interval, in seconds, for providing device-motion updates to the block handler.

func startDeviceMotionUpdates(using: CMAttitudeReferenceFrame, to: OperationQueue, withHandler: CMDeviceMotionHandler)

Starts device-motion updates on an operation queue and using a specified reference frame and block handler.

func startDeviceMotionUpdates(to: OperationQueue, withHandler: CMDeviceMotionHandler)

Starts device-motion updates on an operation queue and using a specified block handler.

func startDeviceMotionUpdates(using: CMAttitudeReferenceFrame)

Starts device-motion updates using a reference frame but without a block handler.

func startDeviceMotionUpdates()

Starts device-motion updates without a block handler.

func stopDeviceMotionUpdates()

Stops device-motion updates.

var deviceMotion: CMDeviceMotion?

The latest sample of device-motion data.

