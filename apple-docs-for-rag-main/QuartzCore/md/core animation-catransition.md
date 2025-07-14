

- Core Animation
-  CATransition 

Class

# CATransition

An object that provides an animated transition between a layer’s states.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CATransition
```

## Overview

You can transition between a layer’s states by creating and adding a CATransition object to it. The default transition is a cross fade, but you can specify different effects from a set of predefined transitions.

The following code shows how you can transition between the two states of a CATextLayer named `transitioningLayer`. When the layer is first created, its backgroundColor is set to red and its string property is set to `Red`. When the `runTransition()` function is called, a new CATransition object is created and added to `transitioningLayer`, and the state of the layer is changed so that its background color is blue and its rendered text reads `Blue`.

The end result is that the push transition animates the red state from left to right with the blue state entering the scene from the left.

```
let transitioningLayer = CATextLayer()

override func viewDidLoad() {
    super.viewDidLoad()
    transitioningLayer.frame = CGRect(x: 10, y: 10,
                                      width: 320, height: 160)

    view.layer.addSublayer(transitioningLayer)

    // Initial "red" state
    transitioningLayer.backgroundColor = UIColor.red.cgColor
    transitioningLayer.string = "Red"
}

func runTransition() {
    let transition = CATransition()
    transition.duration = 2

    transition.type = kCATransitionPush

    transitioningLayer.add(transition,
                           forKey: "transition")

    // Transition to "blue" state
    transitioningLayer.backgroundColor = UIColor.blue.cgColor
    transitioningLayer.string = "Blue"
}
```

## Topics

### Transition start and end point

var startProgress: Float

Indicates the start point of the receiver as a fraction of the entire transition.

var endProgress: Float

Indicates the end point of the receiver as a fraction of the entire transition.

### Transition Properties

var type: CATransitionType

Specifies the predefined transition type.

var subtype: CATransitionSubtype?

Specifies an optional subtype that indicates the direction for the predefined motion-based transitions.

### Custom transition filter

var filter: Any?

An optional Core Image filter object that provides the transition.

### Constants

Common Transition Types

These constants specify the transition types that can be used with the type property.

Common Transition Subtypes

These constants specify the direction of motion-based transitions. They are used with the subtype property.

## Relationships

### Inherits From

- CAAnimation

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

class CASpringAnimation

An animation that applies a spring-like force to a layer’s properties.

class CAValueFunction

An object that provides a flexible method of defining animated transformations.

