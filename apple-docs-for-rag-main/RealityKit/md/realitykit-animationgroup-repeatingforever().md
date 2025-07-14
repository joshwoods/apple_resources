

- RealityKit
- AnimationGroup
-  repeatingForever() 

Instance Method

# repeatingForever()

Repeats the animation infinitely.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
func repeatingForever() -> Self
```

## Return Value

A version of the calling animation that will repeat infinitely.

## See Also

### Repeating group playback

var repeatMode: AnimationRepeatMode

An option that determines how the animations repeat.

var fillMode: AnimationFillMode

An option that determines which data displays outside of the normal duration.

func repeated(count: TimeInterval) -> Self

Repeats an animation the number of times specified by an irrational number.

func repeated(count: Int) -> Self

Repeats an animation the number of times specified by a whole number.

