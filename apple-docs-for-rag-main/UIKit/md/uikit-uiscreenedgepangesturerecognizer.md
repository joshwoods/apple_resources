

- UIKit
-  UIScreenEdgePanGestureRecognizer 

Class

# UIScreenEdgePanGestureRecognizer

A continuous gesture recognizer that interprets panning gestures that start near an edge of the screen.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+

``` source
@MainActor
class UIScreenEdgePanGestureRecognizer
```

## Mentioned in 

Handling pan gestures

## Overview

The system uses screen edge gestures in some cases to initiate view controller transitions. You can use this class to replicate the same gesture behavior for your own actions.

After creating a screen edge pan gesture recognizer, assign an appropriate value to the edges property before attaching the gesture recognizer to your view. You use this property to specify the edges where the gesture can start. This gesture recognizer ignores any touches beyond the first touch.

## Topics

### Specifying the starting edges

var edges: UIRectEdge

The acceptable starting edges for the gesture.

struct UIRectEdge

Constants that specify the edges of a rectangle.

## Relationships

### Inherits From

- UIPanGestureRecognizer

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

class UISwipeGestureRecognizer

A discrete gesture recognizer that interprets swiping gestures in one or more directions.

class UITapGestureRecognizer

A discrete gesture recognizer that interprets single or multiple taps.

