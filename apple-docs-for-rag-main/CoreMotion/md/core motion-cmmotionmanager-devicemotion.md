

- Core Motion
- CMMotionManager
-  deviceMotion 

Instance Property

# deviceMotion

The latest sample of device-motion data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var deviceMotion: CMDeviceMotion? { get }
```

## Mentioned in 

Getting processed device-motion data

## Discussion

If no device-motion data is available, the value of this property is `nil`. An app that is receiving device-motion data after calling startDeviceMotionUpdates() periodically checks the value of this property and processes the device-motion data.

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

typealias CMDeviceMotionHandler

The type of block callback for handling device-motion data.

