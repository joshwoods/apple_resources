

- Core Animation
-  CAKeyframeAnimation 

Class

# CAKeyframeAnimation

An object that provides keyframe animation capabilities for a layer object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CAKeyframeAnimation
```

## Overview

You create a CAKeyframeAnimation object using the inherited init(keyPath:) method, specifying the key path of the property that you want to animate on the layer. You can then specify the keyframe values to use to control the timing and animation behavior.

For most types of animations, you specify the keyframe values using the values and keyTimes properties. During the animation, Core Animation generates intermediate values by interpolating between the values you provide. When animating a value that is a coordinate point, such as the layer’s position, you can specify a path for that point to follow instead of individual values. The pacing of the animation is controlled by the timing information you provide.

The following code shows how to create a keyframe animation that animates a layer’s background color from red to green to blue over a two second duration.

```
let colorKeyframeAnimation = CAKeyframeAnimation(keyPath: "backgroundColor")

colorKeyframeAnimation.values = [UIColor.red.cgColor,
                                 UIColor.green.cgColor,
                                 UIColor.blue.cgColor]
colorKeyframeAnimation.keyTimes = [0, 0.5, 1]
colorKeyframeAnimation.duration = 2
```

## Topics

### Providing keyframe values

var values: [Any]?

An array of objects that specify the keyframe values to use for the animation.

var path: CGPath?

The path for a point-based property to follow.

### Keyframe timing

var keyTimes: [NSNumber]?

An optional array of `NSNumber` objects that define the time at which to apply a given keyframe segment.

var timingFunctions: [CAMediaTimingFunction]?

An optional array of `CAMediaTimingFunction` objects that define the pacing for each keyframe segment.

var calculationMode: CAAnimationCalculationMode

Specifies how intermediate keyframe values are calculated by the receiver.

### Rotation Mode Attribute

var rotationMode: CAAnimationRotationMode?

Determines whether objects animating along the path rotate to match the path tangent.

### Cubic Mode Attributes

var tensionValues: [NSNumber]?

An array of numbers that define the tightness of the curve.

var continuityValues: [NSNumber]?

An array of numbers that define the sharpness of the timing curve’s corners.

var biasValues: [NSNumber]?

An array of numbers that define the position of the curve relative to a control point.

### Constants

Rotation Mode Values

These constants are used by the rotationMode property.

Value calculation modes

These constants are used by the calculationMode property.

## Relationships

### Inherits From

- CAPropertyAnimation

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

class CASpringAnimation

An animation that applies a spring-like force to a layer’s properties.

class CATransition

An object that provides an animated transition between a layer’s states.

class CAValueFunction

An object that provides a flexible method of defining animated transformations.

