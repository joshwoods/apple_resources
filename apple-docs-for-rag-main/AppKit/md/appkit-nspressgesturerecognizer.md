

- AppKit
-  NSPressGestureRecognizer 

Class

# NSPressGestureRecognizer

A discrete gesture recognizer that tracks whether the user holds down a mouse button for a minimum amount of time before releasing it.

macOS 10.10+

``` source
@MainActor
class NSPressGestureRecognizer
```

## Overview

Use a press gesture recognizer to configure which button the user must hold and the length of time they must hold it. You can also specify how far the mouse can move for a valid gesture.

Upon creation, the gesture recognizer recognizes press gestures involving only the primary button. It also delays sending primary button events to the view by setting the delaysPrimaryMouseButtonEvents property to true. To change the set of buttons to track, modify the buttonMask property.

## Topics

### Configuring the Gesture Recognizer

var allowableMovement: CGFloat

The maximum movement of the mouse in the view before the gesture fails.

var buttonMask: Int

A bit mask of the buttons required to recognize this press.

var minimumPressDuration: TimeInterval

The minimum time (in seconds) that the user must hold the mouse button in the view for a valid gesture.

var numberOfTouchesRequired: Int

The number of necessary touches on a Touch Bar for the gesture recognizer to match.

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

class NSPanGestureRecognizer

A continuous gesture recognizer for panning gestures.

class NSRotationGestureRecognizer

A continuous gesture recognizer that tracks two trackpad touches moving opposite each other in a circular motion.

class NSMagnificationGestureRecognizer

A continuous gesture recognizer that tracks a pinch gesture that magnifies content.

