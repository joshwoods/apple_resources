

- RealityKit
- FromToByAnimation
-  delay 

Instance Property

# delay

An amount of time that elapses before the animation plays.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var delay: TimeInterval { get set }
```

## Discussion

The default value is `0`, which indicates that the animation plays with no delay. If you set a value for this property, the animation plays from its start time after the specified delay lapses.

During the delayed time, the animation doesn’t update. However, to fill the delayed time with some portion of animation, set a negative trimStart instead and choose a fillMode that displays the desired portion of animation.

## See Also

### Timing the animation

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

var duration: TimeInterval

The total playback time of the animation.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var timing: AnimationTimingFunction

An option that determines the animation’s pace over time.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The time, in seconds, at which the animation plays.

var trimEnd: TimeInterval?

The time, in seconds, at which the animation stops.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

