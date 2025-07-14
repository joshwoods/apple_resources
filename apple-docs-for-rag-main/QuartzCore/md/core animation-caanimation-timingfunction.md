

- Core Animation
- CAAnimation
-  timingFunction 

Instance Property

# timingFunction

An optional timing function defining the pacing of the animation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var timingFunction: CAMediaTimingFunction? { get set }
```

## Discussion

Defaults to `nil`, indicating linear pacing.

## See Also

### Animation Attributes

var isRemovedOnCompletion: Bool

Determines if the animation is removed from the target layer’s animations upon completion.

