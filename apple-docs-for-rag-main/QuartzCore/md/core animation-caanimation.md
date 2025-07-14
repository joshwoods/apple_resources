

- Core Animation
-  CAAnimation 

Class

# CAAnimation

The abstract superclass for animations in Core Animation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CAAnimation
```

## Mentioned in 

Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro

## Overview

`CAAnimation` provides the basic support for the CAMediaTiming and CAAction protocols. You do not create instance of CAAnimation: to animate Core Animation layers or SceneKit objects, create instances of the concrete subclasses CABasicAnimation, CAKeyframeAnimation, CAAnimationGroup, or CATransition.

### Animating Core Animation Layers

You can animate the contents of your iOS or macOS app’s user interface by attaching animations to CALayer objects. For more information, see Core Animation Programming Guide.

### Animating Scene Kit Content

In Scene Kit, animation objects represent not only property-based animations, but also animations of geometry data created with external 3D authoring tools and loaded from a scene file. You use the properties of the CAAnimation object representing a geometry animation to control its timing, monitor its progress, and attach actions for Scene Kit to trigger during the animation. You can attach animations to Scene Kit objects that adopt the SCNAnimatable protocol, including nodes, geometries, and materials.

In a Scene Kit app, CAAnimation objects support additional methods and properties, listed under Controlling SceneKit Animation Timing, Fading between SceneKit Animations, and Attaching SceneKit Animation Events.

## Topics

### Creating an Animation

init(SCNAnimation: SCNAnimation)

Creates an animation from a SceneKit animation.

### Animation Attributes

var isRemovedOnCompletion: Bool

Determines if the animation is removed from the target layer’s animations upon completion.

var timingFunction: CAMediaTimingFunction?

An optional timing function defining the pacing of the animation.

### Providing Default Values

class func defaultValue(forKey: String) -> Any?

Specifies the default value of the property with the specified key.

### Designating a Delegate

var delegate: (any CAAnimationDelegate)?

Specifies the receiver’s delegate object.

### Archiving Properties

func shouldArchiveValue(forKey: String) -> Bool

Specifies whether the value of the property for a given key is archived.

### Controlling SceneKit Animation Timing

var usesSceneTimeBase: Bool

For animations attached to SceneKit objects, a Boolean value that determines whether the animation is evaluated using the scene time or the system time.

### Fading between SceneKit Animations

var fadeInDuration: CGFloat

For animations attached to SceneKit objects, the duration for transitioning into the animation’s effect as it begins.

var fadeOutDuration: CGFloat

For animations attached to SceneKit objects, the duration for transitioning out of the animation’s effect as it ends.

### Attaching SceneKit Animation Events

var animationEvents: [SCNAnimationEvent]?

For animations attached to SceneKit objects, a list of events attached to an animation.

### Initializers

init(SCNAnimation: SCNAnimation)

Creates an animation from a SceneKit animation.

### Instance Properties

var preferredFrameRateRange: CAFrameRateRange

## Relationships

### Inherits From

- NSObject

### Inherited By

- CAAnimationGroup
- CAPropertyAnimation
- CATransition

### Conforms To

- CAAction
- CAMediaTiming
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- SCNAnimationProtocol

## See Also

### Animation

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

class CAValueFunction

An object that provides a flexible method of defining animated transformations.

