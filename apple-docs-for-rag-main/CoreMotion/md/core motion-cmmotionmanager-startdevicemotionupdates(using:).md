

- Core Motion
- CMMotionManager
-  startDeviceMotionUpdates(using:) 

Instance Method

# startDeviceMotionUpdates(using:)

Starts device-motion updates using a reference frame but without a block handler.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
func startDeviceMotionUpdates(using referenceFrame: CMAttitudeReferenceFrame)
```

## Parameters 

`referenceFrame`  

A constant identifying the reference frame to use for device-motion updates. It’s your responsibility to specify a reference frame that’s available on the current device. Call availableAttitudeReferenceFrames() to determine which reference frames are currently available.

## Discussion

You can get the latest device-motion data through the deviceMotion property. You must call stopDeviceMotionUpdates() when you no longer want your app to process device-motion updates.

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

func startDeviceMotionUpdates()

Starts device-motion updates without a block handler.

func stopDeviceMotionUpdates()

Stops device-motion updates.

var deviceMotion: CMDeviceMotion?

The latest sample of device-motion data.

typealias CMDeviceMotionHandler

The type of block callback for handling device-motion data.

