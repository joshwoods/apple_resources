

- UIKit
-  UISwipeGestureRecognizer 

Class

# UISwipeGestureRecognizer

A discrete gesture recognizer that interprets swiping gestures in one or more directions.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UISwipeGestureRecognizer
```

## Mentioned in 

Handling swipe gestures

## Overview

UISwipeGestureRecognizer is a concrete subclass of UIGestureRecognizer.

UISwipeGestureRecognizer recognizes a swipe when the user moves the specified number of touches (numberOfTouchesRequired) in an allowable direction (direction) far enough to create a swipe. Swipes can be slow or fast. A slow swipe requires high directional precision but a small distance; a fast swipe requires low directional precision but a large distance. Because a swipe is a discrete gesture, the system sends the associated action message just once per gesture.

You can determine the location where a swipe begins by calling the UIGestureRecognizer methods location(in:) and location(ofTouch:in:). The former method provides the centroid if the gesture contains more than one touch; the latter provides the location of a particular touch.

## Topics

### Configuring the gesture

var direction: UISwipeGestureRecognizer.Direction

The permitted direction of the swipe for this gesture recognizer.

var numberOfTouchesRequired: Int

The number of touches necessary for swipe recognition.

struct Direction

The direction of the swipe.

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

class UITapGestureRecognizer

A discrete gesture recognizer that interprets single or multiple taps.

