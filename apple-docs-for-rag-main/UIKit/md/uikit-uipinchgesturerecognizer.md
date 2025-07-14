

- UIKit
-  UIPinchGestureRecognizer 

Class

# UIPinchGestureRecognizer

A continuous gesture recognizer that interprets pinching gestures involving two touches.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIPinchGestureRecognizer
```

## Mentioned in 

Handling pinch gestures

## Overview

UIPinchGestureRecognizer is a concrete subclass of UIGestureRecognizer.

The user must press two fingers on a view while pinching it. When the user moves the two fingers toward each other, the conventional meaning is zoom out; when the user moves the two fingers away from each other, the conventional meaning is zoom in.

Pinching is a continuous gesture. The gesture begins (UIGestureRecognizer.State.began) when the user moves the two fingers enough to create a pinch gesture. The gesture changes (UIGestureRecognizer.State.changed) when a finger moves (while both fingers remain touching). The gesture ends (UIGestureRecognizer.State.ended) when the user lifts both fingers from the view.

## Topics

### Interpreting the pinching gesture

var scale: CGFloat

The scale factor relative to the points of the two touches in screen coordinates.

var velocity: CGFloat

The velocity of the pinch in scale factor per second.

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

class UIRotationGestureRecognizer

A continuous gesture recognizer that interprets rotation gestures involving two touches.

class UIScreenEdgePanGestureRecognizer

A continuous gesture recognizer that interprets panning gestures that start near an edge of the screen.

class UISwipeGestureRecognizer

A discrete gesture recognizer that interprets swiping gestures in one or more directions.

class UITapGestureRecognizer

A discrete gesture recognizer that interprets single or multiple taps.

