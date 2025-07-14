

- UIKit
-  UICubicTimingParameters 

Class

# UICubicTimingParameters

The timing information for animations in the form of a cubic Bézier curve.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class UICubicTimingParameters
```

## Overview

Use a UICubicTimingParameters object to specify custom timing curves when creating animations with objects that adopt the UIViewAnimating protocol, such as UIViewPropertyAnimator.

A cubic Bézier timing curve consists of a line whose starting point is (`0`, `0`), whose end point is (`1`, `1`), and whose shape is defined by two control points. The slope of the line at each point in time defines the speed of the animation at that time. Steep slopes cause animations to appear to run faster and shallower slopes cause them to appear to run slower. The following graph shows a timing curve where the animations start fast and finish fast but run more slowly through the middle section.

## Topics

### Initializing a cubic timing parameters object

init()

Initializes the object with the system’s default timing curve.

init(animationCurve: UIView.AnimationCurve)

Initializes the object with the specified UIKit timing curve.

init(controlPoint1: CGPoint, controlPoint2: CGPoint)

Initializes the object with the specified control points for a cubic Bézier curve.

init?(coder: NSCoder)

Creates a timing parameters object from data in an unarchiver.

### Getting the timing parameters

var animationCurve: UIView.AnimationCurve

The standard UIKit animation curve to use for timing.

var controlPoint1: CGPoint

The first control point for the cubic Bézier curve.

var controlPoint2: CGPoint

The second control point of the cubic Bézier curve.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- Sendable
- UITimingCurveProvider

## See Also

### Timing curves

protocol UITimingCurveProvider

An interface for providing the timing information needed to perform animations.

class UISpringTimingParameters

The timing information for animations that mimics the behavior of a spring.

