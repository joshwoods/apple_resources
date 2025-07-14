

- RealityKit
- OrbitAnimation
-  trimEnd 

Instance Property

# trimEnd

The optional time, in seconds, at which the animation stops.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var trimEnd: TimeInterval? { get set }
```

## Discussion

This property is `nil` by default, which plays the animation until `time` = duration. If you set a value, the animation edits the duration according to the specified ending time.

## See Also

### Timing the animation

var speed: Float

A factor that changes the animation’s rate of playback.

var delay: TimeInterval

An amount of time that lapses before the animation plays.

var duration: TimeInterval

The elapsed time for one complete rotation.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The optional time, in seconds, at which the animation plays.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

