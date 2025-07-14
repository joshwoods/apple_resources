

- UIKit
- UITouch
-  UITouch.Phase 

Enumeration

# UITouch.Phase

The phase of a touch event.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum Phase
```

## Overview

The phase of a `UITouch` instance changes as the system receives updates during the course of an event. Access this value through the phase property.

## Topics

### Constants

case began

A touch for a given event has pressed down on the screen.

case moved

A touch for a given event has moved over the screen.

case stationary

A touch for a given event is pressed down on the screen, but hasn’t moved since the previous event.

case ended

A touch for a given event has lifted from the screen.

case cancelled

The system canceled tracking for a touch, for example, when the user moves the device against their face.

case regionEntered

A touch for a given event has entered a window on the screen.

case regionMoved

A touch for the given event is within a window on the screen, but has not yet pressed down.

case regionExited

A touch for a given event has left a window on the screen.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting touch attributes

var tapCount: Int

The number of times the finger was tapped for this given touch.

var timestamp: TimeInterval

The time when the touch occurred or when it was last mutated.

var type: UITouch.TouchType

The type of the touch.

enum TouchType

The type of touch received.

var phase: UITouch.Phase

The phase of the touch.

var force: CGFloat

The force of the touch, where a value of `1.0` represents the force of an average touch (predetermined by the system, not user-specific).

var maximumPossibleForce: CGFloat

The maximum possible force for a touch.

var altitudeAngle: CGFloat

The altitude (in radians) of the stylus.

func azimuthAngle(in: UIView?) -> CGFloat

Returns the azimuth angle (in radians) of the stylus.

func azimuthUnitVector(in: UIView?) -> CGVector

Returns a unit vector that points in the direction of the azimuth of the stylus.

var rollAngle: CGFloat

A value that represents the current barrel-roll angle of Apple Pencil.

