

- RealityKit
- OrbitAnimation
-  fillMode 

Instance Property

# fillMode

An option that determines which data displays outside of the normal duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var fillMode: AnimationFillMode { get set }
```

## Discussion

This property determines what to display when the framework samples the animation outside of the range defined by its underlying duration. The animation applies this property when:

- Playback progresses toward, but hasn’t yet reached, a nonzero offset. - A range determined by trimStart, trimEnd, or trimDuration exceeds the animation’s underlying duration.

## See Also

### Repeating animation playback

var repeatMode: AnimationRepeatMode

An option that determines how the animation repeats.

func repeated(count: TimeInterval) -> Self

Repeats an animation the number of times specified by an irrational number.

func repeated(count: Int) -> Self

Repeats an animation the number of times specified by a whole number.

func repeatingForever() -> Self

Repeats the animation infinitely.

