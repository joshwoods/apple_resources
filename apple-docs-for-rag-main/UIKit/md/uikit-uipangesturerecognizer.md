

- UIKit
-  UIPanGestureRecognizer 

Class

# UIPanGestureRecognizer

A continuous gesture recognizer that interprets panning gestures.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIPanGestureRecognizer
```

## Mentioned in 

Handling pan gestures

## Overview

UIPanGestureRecognizer is a concrete subclass of UIGestureRecognizer.

Clients of this class can, in their action methods, query the UIPanGestureRecognizer object for the current translation of the gesture (translation(in:)) and the velocity of the translation (velocity(in:)). They can specify a view’s coordinate system to use for the translation and velocity values. Clients can also reset the translation to a desired value.

A panning gesture is continuous. The user must press one or more fingers on a view while panning it. The gesture begins (UIGestureRecognizer.State.began) when the user moves the minimum number of fingers allowed (minimumNumberOfTouches) enough distance for recognition as a pan. It changes (UIGestureRecognizer.State.changed) when the user moves a finger while pressing with the minimum number of fingers. It ends (UIGestureRecognizer.State.ended) when the user lifts all fingers.

## Topics

### Configuring the gesture recognizer

var maximumNumberOfTouches: Int

The maximum number of fingers that can touch the view for gesture recognition.

var minimumNumberOfTouches: Int

The minimum number of fingers that can touch the view for gesture recognition.

### Tracking the location and velocity of the gesture

func translation(in: UIView?) -> CGPoint

Interprets the pan gesture in the coordinate system of the specified view.

func setTranslation(CGPoint, in: UIView?)

Sets the translation value in the coordinate system of the specified view.

func velocity(in: UIView?) -> CGPoint

Interprets the velocity of the pan gesture in the coordinate system of the specified view.

### Tracking scroll events

var allowedScrollTypesMask: UIScrollTypeMask

A scroll type mask that enables recognition of scroll events.

struct UIScrollTypeMask

A bit mask identifying the scroll type of a pan gesture.

enum UIScrollType

Constants that define the type of the scroll.

## Relationships

### Inherits From

- UIGestureRecognizer

### Inherited By

- UIScreenEdgePanGestureRecognizer

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

