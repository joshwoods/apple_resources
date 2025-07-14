

- UIKit
-  UITapGestureRecognizer 

Class

# UITapGestureRecognizer

A discrete gesture recognizer that interprets single or multiple taps.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITapGestureRecognizer
```

## Mentioned in 

Preferring one gesture over another

Handling tap gestures

## Overview

UITapGestureRecognizer is a concrete subclass of UIGestureRecognizer.

For gesture recognition, the specified number of fingers must tap the view a specified number of times. Although taps are discrete gestures, they’re discrete for each state of the gesture recognizer. The system sends the associated action message when the gesture begins and then again for each intermediate state until (and including) the ending state of the gesture. Code that handles tap gestures should test for the state of the gesture, for example:

- Swift
- Objective-C

```
func handleTap(sender: UITapGestureRecognizer) {
    if sender.state == .ended {
        // handling code
    }
}
```

```
- (void)handleTap:(UITapGestureRecognizer *)sender
{
    if (sender.state == UIGestureRecognizerStateEnded)
    {
        // handling code
    }
}
```

Action methods handling this gesture can get the location of the gesture as a whole by calling the UIGestureRecognizer method location(in:). If there are multiple taps, this location is the first tap. If there are multiple touches, this location is the centroid of all fingers tapping the view. Clients can get the location of particular touches in the tap by calling location(ofTouch:in:). If multiple taps are allowed, this location is the first tap.

## Topics

### Configuring the gesture

var buttonMaskRequired: UIEvent.ButtonMask

The bit mask of the buttons the user must press for gesture recognition.

var numberOfTapsRequired: Int

The number of taps necessary for gesture recognition.

var numberOfTouchesRequired: Int

The number of fingers that the user must tap for gesture recognition.

## Relationships

### Inherits From

- UIGestureRecognizer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Standard gestures

Handling UIKit gestures

Use gesture recognizers to simplify touch handling and create a consistent user experience.

Coordinating multiple gesture recognizers

Discover how to use multiple gesture recognizers on the same view.

Adopting hover support for Apple Pencil

Enhance user feedback for your iPadOS app with a hover preview for Apple Pencil input.

Supporting gesture interaction in your apps

Enrich your app’s user experience by supporting standard and custom gesture interaction.

class UIHoverGestureRecognizer

A continuous gesture recognizer that interprets pointer movement over a view.

class UILongPressGestureRecognizer

A continuous gesture recognizer that interprets long-press gestures.

class UIPanGestureRecognizer

A continuous gesture recognizer that interprets panning gestures.

class UIPinchGestureRecognizer

A continuous gesture recognizer that interprets pinching gestures involving two touches.

class UIRotationGestureRecognizer

A continuous gesture recognizer that interprets rotation gestures involving two touches.

class UIScreenEdgePanGestureRecognizer

A continuous gesture recognizer that interprets panning gestures that start near an edge of the screen.

class UISwipeGestureRecognizer

A discrete gesture recognizer that interprets swiping gestures in one or more directions.

