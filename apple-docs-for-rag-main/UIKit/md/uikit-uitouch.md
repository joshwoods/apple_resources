

- UIKit
-  UITouch 

Class

# UITouch

An object representing the location, size, movement, and force of a touch occurring on the screen.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITouch
```

## Mentioned in 

Using responders and the responder chain to handle events

Implementing a Continuous Gesture Recognizer

Implementing a Discrete Gesture Recognizer

Implementing a Multi-Touch app

Computing the perpendicular force of Apple Pencil

## Overview

You access touch objects through UIEvent objects passed into responder objects for event handling. A touch object includes accessors for:

- The view or window in which the touch occurred

- The location of the touch within the view or window

- The approximate radius of the touch

- The force of the touch (on devices that support 3D Touch or Apple Pencil)

A touch object also contains a timestamp indicating when the touch occurred, an integer representing the number of times the user tapped the screen, and the phase of the touch in the form of a constant that describes whether the touch began, moved, or ended, or whether the system canceled the touch.

To learn how to work with swipes, read Handling Swipe and Drag Gestures in Event Handling Guide for UIKit Apps.

A touch object persists throughout a multi-touch sequence. You may store a reference to a touch while handling a multi-touch sequence, as long as you release that reference when the sequence ends. If you need to store information about a touch outside of a multi-touch sequence, copy that information from the touch.

The gestureRecognizers property of a touch contains the gesture recognizers currently handling the touch. Each gesture recognizer is an instance of a concrete subclass of UIGestureRecognizer.

## Topics

### Getting the location of a touch

func location(in: UIView?) -> CGPoint

Returns the current location of the touch in the coordinate system of the given view.

func previousLocation(in: UIView?) -> CGPoint

Returns the previous location of the touch in the coordinate system of the given view.

var view: UIView?

The view to which touches are being delivered, if any.

var window: UIWindow?

The window in which the touch initially occurred.

var majorRadius: CGFloat

The radius (in points) of the touch.

var majorRadiusTolerance: CGFloat

The tolerance (in points) of the touch’s radius.

func preciseLocation(in: UIView?) -> CGPoint

Returns a precise location for the touch, when available.

func precisePreviousLocation(in: UIView?) -> CGPoint

Returns a precise previous location for the touch, when available.

### Getting touch attributes

var tapCount: Int

The number of times the finger was tapped for this given touch.

var timestamp: TimeInterval

The time when the touch occurred or when it was last mutated.

var type: UITouch.TouchType

The type of the touch.

enum TouchType

The type of touch received.

var phase: UITouch.Phase

The phase of the touch.

enum Phase

The phase of a touch event.

var force: CGFloat

The force of the touch, where a value of `1.0` represents the force of an average touch (predetermined by the system, not user-specific).

var maximumPossibleForce: CGFloat

The maximum possible force for a touch.

var altitudeAngle: CGFloat

The altitude (in radians) of the stylus.

func azimuthAngle(in: UIView?) -> CGFloat

Returns the azimuth angle (in radians) of the stylus.

func azimuthUnitVector(in: UIView?) -> CGVector

Returns a unit vector that points in the direction of the azimuth of the stylus.

var rollAngle: CGFloat

A value that represents the current barrel-roll angle of Apple Pencil.

### Managing estimated touch attributes

var estimatedProperties: UITouch.Properties

A set of touch properties whose values contain only estimates.

var estimatedPropertiesExpectingUpdates: UITouch.Properties

The set of touch properties for which updated values are expected in the future.

struct Properties

A bit mask of touch properties that may get updated.

var estimationUpdateIndex: NSNumber?

An index number that lets you correlate an updated touch with the original touch.

### Getting a touch object’s gesture recognizers

var gestureRecognizers: [UIGestureRecognizer]?

The gesture recognizers that are receiving the touch object.

### Working with touch events in SpriteKit

func location(in: SKNode) -> CGPoint

Returns the current location of the touch in the coordinate system of the given node.

func previousLocation(in: SKNode) -> CGPoint

Returns the previous location of the touch in the coordinate system of the given node.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Touches

Handling touches in your view

Use touch events directly on a view subclass if touch handling is intricately linked to the view’s content.

Handling input from Apple Pencil

Learn how to detect and respond to touches from Apple Pencil.

Tracking the force of 3D Touch events

Manipulate your content based on the force of touches.

Illustrating the force, altitude, and azimuth properties of touch input

Capture Apple Pencil and touch input in views.

Leveraging touch input for drawing apps

Capture touches as a series of strokes and render them efficiently on a drawing canvas.

