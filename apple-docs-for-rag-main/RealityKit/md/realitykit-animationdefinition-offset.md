

- RealityKit
- AnimationDefinition
-  offset 

Instance Property

# offset

The time, in seconds, at which the animation begins within the duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var offset: TimeInterval { get set }
```

**Required**

## Discussion

The default value is `0`, which indicates that the animation plays with no offset. Setting a value for this property moves the animation data along the timeline and doesn’t change timing. If you set a fillMode other than none, the animation fills the vacant area created by the offset according to the characteristics of the specified fill mode.

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

