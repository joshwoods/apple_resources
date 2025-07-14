

- Core Motion
- CMMotionManager
-  showsDeviceMovementDisplay 

Instance Property

# showsDeviceMovementDisplay

Controls whether the device-movement display is shown.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var showsDeviceMovementDisplay: Bool { get set }
```

## Discussion

When a device requires movement (for example, to calibrate the compass), the value of this property indicates if the system’s device-movement display should be shown. When a device requires movement, the block handler of type CMDeviceMotionHandler reports the CMErrorDeviceRequiresMovement error once. By default, this property is false.

## See Also

### Managing Device Motion Updates

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

typealias CMDeviceMotionHandler

The type of block callback for handling device-motion data.

