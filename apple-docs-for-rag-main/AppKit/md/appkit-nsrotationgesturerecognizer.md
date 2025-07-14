

- AppKit
-  NSRotationGestureRecognizer 

Class

# NSRotationGestureRecognizer

A continuous gesture recognizer that tracks two trackpad touches moving opposite each other in a circular motion.

macOS 10.10+

``` source
@MainActor
class NSRotationGestureRecognizer
```

## Overview

This rotation gesture implies that the underlying view should rotate in a matching direction. The gesture is recognized when the trackpad touches end.

Upon creation, the gesture recognizer sets the value of the delaysRotationEvents property to true.

## Topics

### Interpreting the Gesture

var rotation: CGFloat

The rotation of the gesture in radians.

var rotationInDegrees: CGFloat

The rotation of the gesture in degrees.

## Relationships

### Inherits From

- NSGestureRecognizer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Standard Gestures

class NSClickGestureRecognizer

A discrete gesture recognizer that tracks a specified number of mouse clicks.

class NSPressGestureRecognizer

A discrete gesture recognizer that tracks whether the user holds down a mouse button for a minimum amount of time before releasing it.

class NSPanGestureRecognizer

A continuous gesture recognizer for panning gestures.

class NSMagnificationGestureRecognizer

A continuous gesture recognizer that tracks a pinch gesture that magnifies content.

