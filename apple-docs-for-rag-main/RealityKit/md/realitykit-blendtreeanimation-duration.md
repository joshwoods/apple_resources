

- RealityKit
- BlendTreeAnimation
-  duration 

Instance Property

# duration

The total playback time of the animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var duration: TimeInterval { get }
```

## Discussion

The framework sets a value for this property depending on the underlying animation data and the specified speed.

You can override the default duration by defining trimStart, trimEnd, or trimDuration.

## See Also

### Timing the animation

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

var delay: TimeInterval

An amount of time that lapses before the animation plays.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The optional time, in seconds, at which the source animation plays.

var trimEnd: TimeInterval?

The optional time, in seconds, at which the source animation stops.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

