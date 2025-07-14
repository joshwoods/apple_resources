

- DockKit
- DockAccessory
-  limits 

Instance Property

# limits

Current limits for the axes of rotation and maximum angular velocity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final var limits: DockAccessory.Limits { get throws }
```

## Return Value

The pitch, yaw, and roll limit. Each value can be `nil` if it’s unsupported. See DockAccessory.Limits for more information.

## Discussion

Throws

DockKitError.notConnected if the device has disconnected.

## See Also

### Getting position and limits

var motionStates: DockAccessory.MotionStates

Motion information from the dock accessory that includes current orientation and velocity of all axes.

struct MotionState

An event that indicates the state of a dock accessory’s current position and speed.

struct MotionStates

An asynchronous sequence of orientation and velocity updates from the device.

struct Limits

Soft limits on multiple axes of rotation.

