

- Core Animation
-  CAPropertyAnimation 

Class

# CAPropertyAnimation

An abstract subclass for creating animations that manipulate the value of layer properties.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CAPropertyAnimation
```

## Overview

The property to animate is specified using a key path that is relative to the layer using the animation.

You do not create instances of CAPropertyAnimation: to animate the properties of a Core Animation layer, create instance of the concrete subclasses CABasicAnimation or CAKeyframeAnimation.

## Topics

### Animated Key Path

var keyPath: String?

Specifies the key path the receiver animates.

### Property Value Calculation Behavior

var isCumulative: Bool

Determines if the value of the property is the value at the end of the previous repeat cycle, plus the value of the current repeat cycle.

var isAdditive: Bool

Determines if the value specified by the animation is added to the current render tree value to produce the new render tree value.

var valueFunction: CAValueFunction?

An optional value function that is applied to interpolated values.

### Creating an Animation

convenience init(keyPath: String?)

Creates and returns an `CAPropertyAnimation` instance for the specified key path.

## Relationships

### Inherits From

- CAAnimation

### Inherited By

- CABasicAnimation
- CAKeyframeAnimation

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

class CABasicAnimation

An object that provides basic, single-keyframe animation capabilities for a layer property.

class CAKeyframeAnimation

An object that provides keyframe animation capabilities for a layer object.

class CASpringAnimation

An animation that applies a spring-like force to a layer’s properties.

class CATransition

An object that provides an animated transition between a layer’s states.

class CAValueFunction

An object that provides a flexible method of defining animated transformations.

