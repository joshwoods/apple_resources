

- RealityKit
- SampledAnimation
-  offset 

Instance Property

# offset

The time, in seconds, at which the animation begins within the duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var offset: TimeInterval { get set }
```

## Discussion

The default value is `0`, which indicates that the animation plays with no offset. Setting a value for this property moves the animation data along the timeline and doesn’t change timing. If you set a fillMode other than none, the animation fills the vacant area created by the offset according to the characteristics of the specified fill mode.

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

var duration: TimeInterval

The total playback time of the animation.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The optional time, in seconds, at which the animation plays.

var trimEnd: TimeInterval?

The optional time, in seconds, at which the animation stops.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

