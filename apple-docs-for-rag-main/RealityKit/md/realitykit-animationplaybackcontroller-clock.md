

- RealityKit
- AnimationPlaybackController
-  clock 

Instance Property

# clock

A reference clock to synchronize the animation with other events.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
var clock: CMClockOrTimebase { get set }
```

## See Also

### Timing animation playback

var duration: TimeInterval

The length of time the animation spans, in seconds.

var speed: Float

The animation’s rate of playback.

var time: TimeInterval

The animation’s location within the timeline.

