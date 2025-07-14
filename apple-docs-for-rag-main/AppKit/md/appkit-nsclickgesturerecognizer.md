

- AppKit
-  NSClickGestureRecognizer 

Class

# NSClickGestureRecognizer

A discrete gesture recognizer that tracks a specified number of mouse clicks.

macOS 10.10+

``` source
@MainActor
class NSClickGestureRecognizer
```

## Overview

When configuring this gesture recognizer, you can specify which mouse buttons must be clicked and how many clicks must occur before the action method is called. The user must click the specified mouse button the required number of times without dragging the mouse for the gesture to be recognized.

The gesture recognizer automatically sets the values of the delaysPrimaryMouseButtonEvents, delaysSecondaryMouseButtonEvents, and delaysOtherMouseButtonEvents properties to true for each button in the buttonMask property.

## Topics

### Configuring the Gesture

var buttonMask: Int

A bit mask of the button (or buttons) required to recognize this click.

var numberOfClicksRequired: Int

The number of clicks required to match.

var numberOfTouchesRequired: Int

The number of touches required in an NSTouchBar object for the gesture recognizer to match.

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

## See Also

### Standard Gestures

class NSPressGestureRecognizer

A discrete gesture recognizer that tracks whether the user holds down a mouse button for a minimum amount of time before releasing it.

class NSPanGestureRecognizer

A continuous gesture recognizer for panning gestures.

class NSRotationGestureRecognizer

A continuous gesture recognizer that tracks two trackpad touches moving opposite each other in a circular motion.

class NSMagnificationGestureRecognizer

A continuous gesture recognizer that tracks a pinch gesture that magnifies content.

