

- RealityKit
- FromToByAnimation
-  trimDuration 

Instance Property

# trimDuration

An optional duration that overrides the calculated duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var trimDuration: TimeInterval? { get set }
```

## Discussion

The framework calculates duration, but you can set this property to override it. This property is `nil` by default, which indicates that the animation stops after one play that spans duration.

If you set a value for this property and both trimStart and trimEnd are `nil`, the animation observes this property as an edited duration.

A value greater than duration causes the animation to repeat, applying the characteristics defined by repeatMode. Assign this property greatestFiniteMagnitude to repeat indefinitely.

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

var timing: AnimationTimingFunction

An option that determines the animation’s pace over time.

var trimStart: TimeInterval?

The time, in seconds, at which the animation plays.

var trimEnd: TimeInterval?

The time, in seconds, at which the animation stops.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

