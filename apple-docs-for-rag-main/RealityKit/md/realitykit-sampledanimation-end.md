

- RealityKit
- SampledAnimation
-  end 

Instance Property

# end

An integer multiple of the frame interval at which the animation stops.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var end: TimeInterval { get set }
```

## Discussion

When calculating the visual beginning of a sampled animation, the framework first evaluates this property, and then applies the optional trimEnd, in seconds.

The framework requires this property to contain an integer multiple of frameInterval. Note that the value of this property can be irrational because frame interval is of type TimeInterval.

## See Also

### Timing the animation

var frameInterval: Float

The duration within the animation timeline for each frame in the frames array.

var start: TimeInterval

An integer multiple of the frame interval at which the animation plays.

var speed: Float

A factor that changes the animation’s rate of playback.

var delay: TimeInterval

An amount of time that elapses before the animation plays.

var duration: TimeInterval

The total playback time of the animation.

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

