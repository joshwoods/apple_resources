

- RealityKit
- SampledAnimation
-  trimDuration 

Instance Property

# trimDuration

An optional duration that overrides the calculated duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var trimDuration: TimeInterval? { get set }
```

## Discussion

This property is `nil` by default, which indicates that the animation stops after one play that spans duration.

If you set a value for this property and both trimStart and trimEnd are `nil`, the animation observes this property as an edited duration.

A value greater than duration causes the animation to repeat, applying the characteristics defined by repeatMode. Assign this property greatestFiniteMagnitude to repeat indefinitely.

## See Also

### Timing the animation

var frameInterval: Float

The duration within the animation timeline for each frame in the frames array.

var start: TimeInterval

An integer multiple of the frame interval at which the animation plays.

var end: TimeInterval

An integer multiple of the frame interval at which the animation stops.

var speed: Float

A factor that changes the animation’s rate of playback.

var delay: TimeInterval

An amount of time that elapses before the animation plays.

var duration: TimeInterval

The total playback time of the animation.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var trimStart: TimeInterval?

The optional time, in seconds, at which the animation plays.

var trimEnd: TimeInterval?

The optional time, in seconds, at which the animation stops.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

