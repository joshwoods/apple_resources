

- DockKit
- DockAccessory
-  DockAccessory.Limits 

Structure

# DockAccessory.Limits

Soft limits on multiple axes of rotation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Limits
```

## Topics

### Creating limits

init(yaw: DockAccessory.Limits.Limit?, pitch: DockAccessory.Limits.Limit?, roll: DockAccessory.Limits.Limit?)

Creates the limit object.

### Specifying limits

struct Limit

A description of a limit placed on an axis of rotation.

### Getting properties

let pitch: DockAccessory.Limits.Limit?

The up and down limit.

let roll: DockAccessory.Limits.Limit?

The side to side limit.

let yaw: DockAccessory.Limits.Limit?

The left and right limit.

## Relationships

### Conforms To

- Sendable

## See Also

### Getting position and limits

var motionStates: DockAccessory.MotionStates

Motion information from the dock accessory that includes current orientation and velocity of all axes.

var limits: DockAccessory.Limits

Current limits for the axes of rotation and maximum angular velocity.

struct MotionState

An event that indicates the state of a dock accessory’s current position and speed.

struct MotionStates

An asynchronous sequence of orientation and velocity updates from the device.

