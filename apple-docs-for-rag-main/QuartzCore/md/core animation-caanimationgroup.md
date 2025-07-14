

- Core Animation
-  CAAnimationGroup 

Class

# CAAnimationGroup

An object that allows multiple animations to be grouped and run concurrently.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CAAnimationGroup
```

## Overview

The grouped animations run in the time space specified by the CAAnimationGroup instance.

The duration of the grouped animations are not scaled to the duration of their CAAnimationGroup. Instead, the animations are clipped to the duration of the animation group. For example, a 10 second animation grouped within an animation group with a duration of 5 seconds displays only the first 5 seconds of the animation.

The following code shows how you can create a grouped animation containing opacity and scale animations to fade out a layer while expanding it. The animation starts with an opacity of `1` and a scale of `1` on all axes. As the animation’s scale increases to `(3, 3, 3)`, the opacity drops to `0` and the animated layer vanishes.

```
let fadeOut = CABasicAnimation(keyPath: "opacity")
fadeOut.fromValue = 1
fadeOut.toValue = 0
fadeOut.duration = 1

let expandScale = CABasicAnimation()
expandScale.keyPath = "transform"
expandScale.valueFunction = CAValueFunction(name: kCAValueFunctionScale)
expandScale.fromValue = [1, 1, 1]
expandScale.toValue = [3, 3, 3]

let fadeAndScale = CAAnimationGroup()
fadeAndScale.animations = [fadeOut, expandScale]
fadeAndScale.duration = 1
```

Important

The delegate and isRemovedOnCompletion properties of animations in the animations array are currently ignored. The CAAnimationGroup delegate does receive these messages.

## Topics

### Grouped animations

var animations: [CAAnimation]?

An array of `CAAnimation` objects to be evaluated in the time space of the receiver.

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

### Animation Groups

class CATransaction

A mechanism for grouping multiple layer-tree operations into atomic updates to the render tree.

