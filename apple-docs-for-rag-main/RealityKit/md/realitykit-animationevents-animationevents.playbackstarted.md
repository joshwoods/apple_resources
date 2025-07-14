

- RealityKit
- AnimationEvents
-  AnimationEvents.PlaybackStarted 

Structure

# AnimationEvents.PlaybackStarted

The event raised when an animation has been started.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct PlaybackStarted
```

## Topics

### Instance Properties

let playbackController: AnimationPlaybackController

The animation playback controller managing the animation that triggered the event.

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Recognizing animation events

struct PlaybackCompleted

The event raised when an animation reaches the end of its duration.

struct PlaybackLooped

The event raised when an animation loops.

struct PlaybackTerminated

The event raised when an animation has been terminated, regardless of whether it ran to completion.

