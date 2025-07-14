

- Core Animation
- CAAnimation
-  isRemovedOnCompletion 

Instance Property

# isRemovedOnCompletion

Determines if the animation is removed from the target layer’s animations upon completion.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var isRemovedOnCompletion: Bool { get set }
```

## Discussion

When true, the animation is removed from the target layer’s animations once its active duration has passed. Defaults to true.

## See Also

### Animation Attributes

var timingFunction: CAMediaTimingFunction?

An optional timing function defining the pacing of the animation.

