

- Core Motion
- CMMotionManager
-  startDeviceMotionUpdates(to:withHandler:) 

Instance Method

# startDeviceMotionUpdates(to:withHandler:)

Starts device-motion updates on an operation queue and using a specified block handler.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
func startDeviceMotionUpdates(
    to queue: OperationQueue,
    withHandler handler: @escaping CMDeviceMotionHandler
)
```

## Parameters 

`queue`  

An operation queue provided by the caller. Because the processed events might arrive at a high rate, using the main operation queue is not recommended.

`handler`  

A block that is invoked with each update to handle new device-motion data. The block must conform to the CMDeviceMotionHandler type.

## Discussion

This method reports motion relative to the reference frame in the attitudeReferenceFrame property. You must call stopDeviceMotionUpdates() when you no longer want your app to process device-motion updates.

## See Also

### Managing Device Motion Updates

var showsDeviceMovementDisplay: Bool

Controls whether the device-movement display is shown.

var deviceMotionUpdateInterval: TimeInterval

The interval, in seconds, for providing device-motion updates to the block handler.

func startDeviceMotionUpdates(using: CMAttitudeReferenceFrame, to: OperationQueue, withHandler: CMDeviceMotionHandler)

Starts device-motion updates on an operation queue and using a specified reference frame and block handler.

func startDeviceMotionUpdates(using: CMAttitudeReferenceFrame)

Starts device-motion updates using a reference frame but without a block handler.

func startDeviceMotionUpdates()

Starts device-motion updates without a block handler.

func stopDeviceMotionUpdates()

Stops device-motion updates.

var deviceMotion: CMDeviceMotion?

The latest sample of device-motion data.

typealias CMDeviceMotionHandler

The type of block callback for handling device-motion data.

