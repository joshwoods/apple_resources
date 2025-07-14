

- UIKit
-  UISpringTimingParameters 

Class

# UISpringTimingParameters

The timing information for animations that mimics the behavior of a spring.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class UISpringTimingParameters
```

## Overview

The timing provided by a UISpringTimingParameters object mimics the behavior of a spring acting on the value of the property being animated. This property’s value accelerates toward its final value according to the relative force of the spring, which you configure. It then oscillates around that final value until it comes to a rest. The speed at which a property animates to its new value is based on the initial velocity of the value and the damping ratio applied to the spring. You can specify those values directly or using analogous spring-related values.

Use instances of this class to specify custom timing curves when creating animations with objects that adopt the UIViewAnimating protocol, such as UIViewPropertyAnimator. Spring animations are commonly used to modify a view’s position onscreen, but you can apply the timing to any of the view’s properties to get a similar type of animation timing.

## Topics

### Initializing a spring timing parameters object

init()

Creates a default timing parameters object.

convenience init(dampingRatio: CGFloat)

Creates a timing parameters object with the specified damping ratio.

init(dampingRatio: CGFloat, initialVelocity: CGVector)

Creates a timing parameters object with the specified damping ratio and initial velocity.

init(mass: CGFloat, stiffness: CGFloat, damping: CGFloat, initialVelocity: CGVector)

Creates a timing parameters object with the specified spring stiffness, mass, damping coefficient, and initial velocity.

init?(coder: NSCoder)

Creates a timing parameters object from data in an unarchiver.

### Getting the initial velocity

var initialVelocity: CGVector

The target property’s rate of change at the start of a spring animation, enabling a smooth transition into the animation.

### Initializers

convenience init(duration: TimeInterval, bounce: CGFloat)

init(duration: TimeInterval, bounce: CGFloat, initialVelocity: CGVector)

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

class UICubicTimingParameters

The timing information for animations in the form of a cubic Bézier curve.

