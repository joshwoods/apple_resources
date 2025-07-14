

- Core Animation
-  CABasicAnimation 

Class

# CABasicAnimation

An object that provides basic, single-keyframe animation capabilities for a layer property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CABasicAnimation
```

## Overview

You create an instance of CABasicAnimation using the inherited init(keyPath:) method, specifying the key path of the property to be animated in the render tree.

For example, you can animate a layer’s scalar (i.e. containing a single value) properties such as its opacity. The following code fades in a layer by animating its opacity from `0` to `1`.

```
let animation = CABasicAnimation(keyPath: "opacity") 
animation.fromValue = 0 
animation.toValue = 1
```

Non-scalar properties, such as backgroundColor, can also be animated. Core Animation will interpolate between the fromValue color and the toValue color. The animation created in the following code fades a layer’s background color from red to blue.

```
let animation = CABasicAnimation(keyPath: "backgroundColor")
animation.fromValue = NSColor.red.cgColor
animation.toValue = NSColor.blue.cgColor
```

If you want to animate the individual components of a non-scalar property with different values, you pass the values to toValue and fromValue as arrays. The following animation moves a layer from `(0, 0)` to `(100, 100)`.

```
let animation = CABasicAnimation(keyPath: "position")
animation.fromValue = [0, 0]
animation.toValue = [100, 100]
```

The `keyPath` can access the individual components of a property. For example, the following animation stretches a layer by animating its transform object’s `x` from `1` to `2`.

```
let animation = CABasicAnimation(keyPath: "transform.scale.x")
animation.fromValue = 1
animation.toValue = 2
```

### Setting Interpolation Values

The fromValue, byValue and toValue properties define the values being interpolated between. All are optional, and no more than two should be non-`nil`. The object type should match the type of the property being animated.

The interpolation values are used as follows:

- Both fromValue and toValue are non-`nil`. Interpolates between fromValue and toValue.

- fromValue and byValue are non-`nil`. Interpolates between fromValue and (fromValue + byValue).

- byValue and toValue are non-`nil`. Interpolates between (toValue - byValue) and toValue.

- fromValue is non-`nil`. Interpolates between fromValue and the current presentation value of the property.

- toValue is non-`nil`. Interpolates between the current value of `keyPath` in the target layer’s presentation layer and toValue.

- byValue is non-`nil`. Interpolates between the current value of `keyPath` in the target layer’s presentation layer and that value plus byValue.

- All properties are `nil`. Interpolates between the previous value of `keyPath` in the target layer’s presentation layer and the current value of `keyPath` in the target layer’s presentation layer.

## Topics

### Interpolation values

var fromValue: Any?

Defines the value the receiver uses to start interpolation.

var toValue: Any?

Defines the value the receiver uses to end interpolation.

var byValue: Any?

Defines the value the receiver uses to perform relative interpolation.

## Relationships

### Inherits From

- CAPropertyAnimation

### Inherited By

- CASpringAnimation

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

class CAKeyframeAnimation

An object that provides keyframe animation capabilities for a layer object.

class CASpringAnimation

An animation that applies a spring-like force to a layer’s properties.

class CATransition

An object that provides an animated transition between a layer’s states.

class CAValueFunction

An object that provides a flexible method of defining animated transformations.

