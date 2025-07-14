

- Core Animation
-  CASpringAnimation 

Class

# CASpringAnimation

An animation that applies a spring-like force to a layer’s properties.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class CASpringAnimation
```

## Overview

You would typically use a spring animation to animate a layer’s position so that it appears to be pulled towards a target by a spring. The further the layer is from the target, the greater the acceleration towards it is.

CASpringAnimation allows control over physically based attributes such as the spring’s damping and stiffness.

You can use a spring animation to animation properties of a layer other than its position. The following code shows how to create a spring animation that bounces a layer into view by animating its scale from `0` to `1`. Because the spring animation can overshoot its toValue, the animated layer may exceed its frame.

```
let springAnimation = CASpringAnimation(keyPath: "transform.scale")

springAnimation.fromValue = 0
springAnimation.toValue = 1
```

## Topics

### Configuring Physical Attributes

var damping: CGFloat

Defines how the spring’s motion should be damped due to the forces of friction.

var initialVelocity: CGFloat

The initial velocity of the object attached to the spring.

var mass: CGFloat

The mass of the object attached to the end of the spring.

var settlingDuration: CFTimeInterval

The estimated duration required for the spring system to be considered at rest.

var stiffness: CGFloat

The spring stiffness coefficient.

### Initializers

init(perceptualDuration: CFTimeInterval, bounce: CGFloat)

### Instance Properties

var allowsOverdamping: Bool

var bounce: CGFloat

var perceptualDuration: CFTimeInterval

## Relationships

### Inherits From

- CABasicAnimation

### Conforms To

- CAAction
- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Animation

class CAAnimation

The abstract superclass for animations in Core Animation.

protocol CAAnimationDelegate

Methods your app can implement to respond when animations start and stop.

class CAPropertyAnimation

An abstract subclass for creating animations that manipulate the value of layer properties.

class CABasicAnimation

An object that provides basic, single-keyframe animation capabilities for a layer property.

class CAKeyframeAnimation

An object that provides keyframe animation capabilities for a layer object.

class CATransition

An object that provides an animated transition between a layer’s states.

class CAValueFunction

An object that provides a flexible method of defining animated transformations.

