

- AppKit
-  NSMagnificationGestureRecognizer 

Class

# NSMagnificationGestureRecognizer

A continuous gesture recognizer that tracks a pinch gesture that magnifies content.

macOS 10.10+

``` source
@MainActor
class NSMagnificationGestureRecognizer
```

## Overview

This object tracks pinch gestures on a track pad or other input device and stores the resulting magnification value for you to use in your code.

This gesture recognizer automatically sets the value of the delaysMagnificationEvents property to true.

## Topics

### Finding the Magnification Factor

var magnification: CGFloat

The amount of magnification to apply.

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

class NSRotationGestureRecognizer

A continuous gesture recognizer that tracks two trackpad touches moving opposite each other in a circular motion.

