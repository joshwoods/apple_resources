

- Core Animation
-  CAAnimationDelegate 

Protocol

# CAAnimationDelegate

Methods your app can implement to respond when animations start and stop.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
protocol CAAnimationDelegate : NSObjectProtocol
```

## Overview

You can use an animation delegate to execute additional logic when an animation starts or ends. For example, you may want to remove a layer from its parent once a fade out animation has completed.

The following example shows code taken from a class that implements CAAnimationDelegate and has had a layer, named `sublayer`, added to its layer. The `fadeOut` function animates the opacity of `sublayer` and, once the animation has completed, animationDidStop(_:finished:) removes it from its superlayer.

```
```

## Topics

### Customizing Start and Stop Times

func animationDidStart(CAAnimation)

Tells the delegate the animation has started.

func animationDidStop(CAAnimation, finished: Bool)

Tells the delegate the animation has ended.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Animation

class CAAnimation

The abstract superclass for animations in Core Animation.

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

