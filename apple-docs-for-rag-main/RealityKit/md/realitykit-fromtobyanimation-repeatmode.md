

- RealityKit
- FromToByAnimation
-  repeatMode 

Instance Property

# repeatMode

An option that determines how the animation repeats.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var repeatMode: AnimationRepeatMode { get set }
```

## Discussion

If you call trimmed(start:end:duration:) with a `start` or `end` that lies outside of the timeline defined by duration, the animation fills the additional playback by applying this property.

## See Also

### Repeating animation playback

var fillMode: AnimationFillMode

An option that determines which data displays outside of the normal duration.

func repeated(count: TimeInterval) -> Self

Repeats an animation the number of times specified by an irrational number.

func repeated(count: Int) -> Self

Repeats an animation the number of times specified by a whole number.

func repeatingForever() -> Self

Repeats the animation infinitely.

