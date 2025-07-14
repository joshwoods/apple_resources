

- UIKit
-  UILongPressGestureRecognizer 

Class

# UILongPressGestureRecognizer

A continuous gesture recognizer that interprets long-press gestures.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UILongPressGestureRecognizer
```

## Overview

UILongPressGestureRecognizer is a concrete subclass of UIGestureRecognizer.

The user must press one or more fingers on a view and hold them there for a minimum period of time before the action triggers. While down, the userʼs fingers canʼt move more than a specified distance or the gesture fails.

A long-press gesture is continuous. The gesture begins (UIGestureRecognizer.State.began) when the user presses the number of allowable fingers (numberOfTouchesRequired) for the specified period (minimumPressDuration) and the touches don’t move beyond the allowable range of movement (allowableMovement). The gesture recognizer transitions to the Change state whenever a finger moves, and it ends (UIGestureRecognizer.State.ended) when the user lifts any of the fingers.

## Topics

### Configuring the gesture recognizer

var minimumPressDuration: TimeInterval

The minimum time that the user must press on the view for the gesture to be recognized.

var numberOfTouchesRequired: Int

The number of fingers that must touch the view for gesture recognition.

var numberOfTapsRequired: Int

The number of taps on the view necessary for gesture recognition.

var allowableMovement: CGFloat

The maximum movement of the fingers on the view before the gesture fails.

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

class UITapGestureRecognizer

A discrete gesture recognizer that interprets single or multiple taps.

