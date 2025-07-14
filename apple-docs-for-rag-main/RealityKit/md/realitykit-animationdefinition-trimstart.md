

- RealityKit
- AnimationDefinition
-  trimStart 

Instance Property

# trimStart

The time, in seconds, at which the animation plays.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var trimStart: TimeInterval? { get set }
```

**Required**

## Discussion

This property is `nil` by default, which plays the animation with `time` = `0`. If you set a value, the animation edits the duration according to the specified beginning time.

If you set a negative value for this property, the duration increases and the additional animation data fills in based on the fillMode you choose.

## See Also

### Timing the animation

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

**Required**

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

var trimEnd: TimeInterval?

The time, in seconds, at which the source animation stops.

**Required**

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

