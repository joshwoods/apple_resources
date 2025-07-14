

- Core Animation
-  CAValueFunction 

Class

# CAValueFunction

An object that provides a flexible method of defining animated transformations.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
class CAValueFunction
```

## Overview

You can use a value function to specify the individual components of an animated transform.

For example, to create a basic animation that rotates a layer from 0° to 180° around its z-axis, you would create a CABasicAnimation object with a fromValue of `0`, a toValue of pi, and a valueFunction of a CAValueFunction with a function name of rotateZ.

The following code shows how you would create such a rotation and apply it to a CALayer named `rotatingLayer`.

```
let rotateAnimation = CABasicAnimation()
rotateAnimation.valueFunction = CAValueFunction(name: kCAValueFunctionRotateZ)
rotateAnimation.fromValue = 0
rotateAnimation.toValue = Float.pi
rotateAnimation.duration = 3
rotatingLayer.add(rotateAnimation,
                  forKey: "transform")
```

The value functions scale and translate require 3 values, for the individual `x`, `y` and `z` components. When working with these value functions, you specify the animation’s fromValue and toValue as arrays.

The following code shows how you could animate a layer’s scale from `0` to `1` using a value function.

```
let scaleAnimation = CABasicAnimation()
scaleAnimation.valueFunction = CAValueFunction(name: kCAValueFunctionScale)
scaleAnimation.fromValue = [0, 0, 0]
scaleAnimation.toValue = [1, 1, 1]
scaleAnimation.duration = 3
scalingLayer.add(scaleAnimation,
                 forKey: "transform")
```

## Topics

### Getting Value Function Properties

var name: CAValueFunctionName

Returns the name of the value function.

### Creating and Initializing Value Functions

convenience init?(name: CAValueFunctionName)

Returns the value function object identified by the name.

### Constants

Rotate Value Functions

Rotate value transform functions construct a 4x4 matrix that represents the corresponding rotation matrix.

Scale Value Functions

Scale value transform functions construct a 4x4 matrix that represents the corresponding scale matrix.

Translate Functions

Translate value transform functions construct a 4x4 matrix that represents the corresponding translate matrix.

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

class CASpringAnimation

An animation that applies a spring-like force to a layer’s properties.

class CATransition

An object that provides an animated transition between a layer’s states.

