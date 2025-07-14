

- DockKit
- DockAccessory
-  DockAccessory.MotionState 

Structure

# DockAccessory.MotionState

An event that indicates the state of a dock accessory’s current position and speed.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct MotionState
```

## Overview

This event indicates the dock accessory’s current velocity and position along each supported axis of rotation. For more information, see motionStates.

## Topics

### Getting properties

let angularPositions: Vector3D

The angles of the axes, in radians.

let angularVelocities: Vector3D

The angular velocity of each axis of rotation in radians.

let timestamp: TimeInterval

The current time, in UNIX epoch.

let error: (any Error)?

The error, if any.

## Relationships

### Conforms To

- Sendable

## See Also

### Getting position and limits

var motionStates: DockAccessory.MotionStates

Motion information from the dock accessory that includes current orientation and velocity of all axes.

var limits: DockAccessory.Limits

Current limits for the axes of rotation and maximum angular velocity.

struct MotionStates

An asynchronous sequence of orientation and velocity updates from the device.

struct Limits

Soft limits on multiple axes of rotation.

