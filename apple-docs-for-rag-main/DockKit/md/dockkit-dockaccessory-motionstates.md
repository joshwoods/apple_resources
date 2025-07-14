

- DockKit
- DockAccessory
-  motionStates 

Instance Property

# motionStates

Motion information from the dock accessory that includes current orientation and velocity of all axes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final var motionStates: DockAccessory.MotionStates { get throws }
```

## Return Value

Motion states with the current orientation and velocity. The dock accessory controls the rate at which the state changes.

## Discussion

This value holds a DockAccessory.MotionStates object, an asynchronous iterator used to find the desired dock accessory.

Throws

DockKitError.notConnected if device is disconnected, or DockKitError.notSupportedByDevice if device doesn’t support updates.

## See Also

### Getting position and limits

var limits: DockAccessory.Limits

Current limits for the axes of rotation and maximum angular velocity.

struct MotionState

An event that indicates the state of a dock accessory’s current position and speed.

struct MotionStates

An asynchronous sequence of orientation and velocity updates from the device.

struct Limits

Soft limits on multiple axes of rotation.

