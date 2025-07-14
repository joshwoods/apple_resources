

- AppKit
-  NSPanGestureRecognizer 

Class

# NSPanGestureRecognizer

A continuous gesture recognizer for panning gestures.

macOS 10.10+

``` source
@MainActor
class NSPanGestureRecognizer
```

## Overview

The gesture is recognized when the user clicks all of specified buttons, drags the mouse, and releases one or more of the buttons. Use the pan gesture recognizer object to retrieve the distance traveled during the pan and the location of the mouse as it pans.

Upon creation, the gesture recognizer is configured to recognize pan gestures involving only the primary button. It also delays sending primary button events to the view by setting the delaysPrimaryMouseButtonEvents property to true. To change the set of buttons to track, modify the buttonMask property.

In this gesture recognizer, the location(in:) method always reports the current mouse point, which changes as the user drags the mouse.

## Topics

### Configuring the Gesture Recognizer

var buttonMask: Int

A bit mask of the button (or buttons) required to recognize this gesture.

var numberOfTouchesRequired: Int

The number of necessary touches on a Touch Bar for the gesture recognizer to match.

### Tracking the Location and Velocity of the Gesture

func translation(in: NSView?) -> NSPoint

The distance traveled by the mouse during the gesture.

func setTranslation(NSPoint, in: NSView?)

Changes the current translation value of the gesture recognizer.

func velocity(in: NSView?) -> NSPoint

The velocity of the pan, measured in points per second.

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

class NSRotationGestureRecognizer

A continuous gesture recognizer that tracks two trackpad touches moving opposite each other in a circular motion.

class NSMagnificationGestureRecognizer

A continuous gesture recognizer that tracks a pinch gesture that magnifies content.

