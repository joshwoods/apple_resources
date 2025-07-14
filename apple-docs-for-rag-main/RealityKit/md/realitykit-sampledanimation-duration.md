

- RealityKit
- SampledAnimation
-  duration 

Instance Property

# duration

The total playback time of the animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var duration: TimeInterval { get set }
```

## Discussion

The framework sets a value for this property depending on the underlying animation data and the specified speed.

You can override the default duration by defining trimStart, trimEnd, or trimDuration.

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

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The optional time, in seconds, at which the animation plays.

var trimEnd: TimeInterval?

The optional time, in seconds, at which the animation stops.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

