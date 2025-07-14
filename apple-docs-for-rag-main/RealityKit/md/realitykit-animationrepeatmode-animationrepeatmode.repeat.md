

- RealityKit
- AnimationRepeatMode
-  AnimationRepeatMode.repeat 

Case

# AnimationRepeatMode.repeat

A mode that restarts the animation after it completes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case `repeat`
```

## Discussion

This mode restores the animated property to its initial value each time it restarts. For example, a FromToByAnimation with fromValue `=` `1.0`, toValue `=` `2.0` and repeatMode set to this property repeats as, `1.0`, `2.0`, `1.0`, `2.0`, `1.0`, `2.0` and so on.

## See Also

### Choosing a repeat mode

case cumulative

A mode that repeats indefinitely and begins each repetition by setting the animated property to the ending value of the previous repetition.

case autoReverse

A mode that reverses the animation after reaching the end or the beginning.

case none

An option that determines the animation doesn’t repeat.

