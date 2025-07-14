

- RealityKit
- FromToByAnimation
-  timing 

Instance Property

# timing

An option that determines the animation’s pace over time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var timing: AnimationTimingFunction { get set }
```

## Discussion

Depending on the option you pick, the animation’s progress moves at varying speeds along its duration.

## See Also

### Timing the animation

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

var delay: TimeInterval

An amount of time that elapses before the animation plays.

var duration: TimeInterval

The total playback time of the animation.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The time, in seconds, at which the animation plays.

var trimEnd: TimeInterval?

The time, in seconds, at which the animation stops.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

