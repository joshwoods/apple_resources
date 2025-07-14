

- RealityKit
- AnimationRepeatMode
-  AnimationRepeatMode.cumulative 

Case

# AnimationRepeatMode.cumulative

A mode that repeats indefinitely and begins each repetition by setting the animated property to the ending value of the previous repetition.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case cumulative
```

## Discussion

A FromToByAnimation with a fromValue of `1.0` and an toValue of `2.0` and repeatMode set to this property repeats as, `1.0`, `2.0`, 3`.0`, 4`.0`, `5.0`, and so on.

## See Also

### Choosing a repeat mode

case `repeat`

A mode that restarts the animation after it completes.

case autoReverse

A mode that reverses the animation after reaching the end or the beginning.

case none

An option that determines the animation doesn’t repeat.

