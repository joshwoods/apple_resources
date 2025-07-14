

- RealityKit
- BlendTreeAnimation
-  repeated(count:) 

Instance Method

# repeated(count:)

Repeats an animation the number of times specified by an irrational number.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
func repeated(count: TimeInterval) -> Self
```

## Parameters 

`count`  

The number of times the animation repeats before stopping.

## Return Value

A version of the calling animation repeated the given number of times.

## See Also

### Repeating animation playback

var repeatMode: AnimationRepeatMode

An option that determines how the animation repeats.

var fillMode: AnimationFillMode

An option that determines which data displays outside of the normal duration.

func repeated(count: Int) -> Self

Repeats an animation the number of times specified by a whole number.

func repeatingForever() -> Self

Repeats the animation infinitely.

