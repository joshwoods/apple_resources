

- UIKit
-  UIRotationGestureRecognizer 

Class

# UIRotationGestureRecognizer

A continuous gesture recognizer that interprets rotation gestures involving two touches.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIRotationGestureRecognizer
```

## Mentioned in 

Handling rotation gestures

## Overview

UIRotationGestureRecognizer is a concrete subclass of UIGestureRecognizer.

The user must press two fingers on a view while rotating it. When the user moves the fingers opposite each other in a circular motion, the underlying view rotates in a corresponding direction and speed.

Rotation is a continuous gesture. It begins when the user moves the two fingers enough to create a rotation gesture. The gesture changes when a finger moves while both fingers remain touching. It ends when the user lifts both fingers. At each stage in the gesture, the gesture recognizer sends its action message.

## Topics

### Interpreting the gesture

var rotation: CGFloat

The rotation of the gesture in radians.

var velocity: CGFloat

The velocity of the rotation gesture in radians per second.

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

class UIScreenEdgePanGestureRecognizer

A continuous gesture recognizer that interprets panning gestures that start near an edge of the screen.

class UISwipeGestureRecognizer

A discrete gesture recognizer that interprets swiping gestures in one or more directions.

class UITapGestureRecognizer

A discrete gesture recognizer that interprets single or multiple taps.

