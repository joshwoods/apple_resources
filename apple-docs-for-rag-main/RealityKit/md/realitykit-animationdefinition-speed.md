

- RealityKit
- AnimationDefinition
-  speed 

Instance Property

# speed

A factor that increases or decreases the animation’s rate of playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var speed: Float { get set }
```

**Required**

## Discussion

The default value is `1.0`, which doesn’t alter the animation’s duration. A value of `2.0` indicates that the duration is half the normal rate. A value of `0.5` indicates that the duration is twice the normal rate. Negative values play the animation in reverse.

This property doesn’t affect the animation’s delay.

## See Also

### Timing the animation

var delay: TimeInterval

An amount of time that elapses before the animation plays.

**Required**

var duration: TimeInterval

The total playback time of the animation.

**Required**

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

**Required**

var trimDuration: TimeInterval?

An optional duration that overrides the source animation’s duration.

**Required**

var trimStart: TimeInterval?

The time, in seconds, at which the animation plays.

**Required**

var trimEnd: TimeInterval?

The time, in seconds, at which the source animation stops.

**Required**

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

