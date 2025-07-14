

- RealityKit
- AnimationEvents
-  AnimationEvents.PlaybackCompleted 

Structure

# AnimationEvents.PlaybackCompleted

The event raised when an animation reaches the end of its duration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct PlaybackCompleted
```

## Overview

This event isn’t triggered if you call the stop() method on a playback controller.

## Topics

### Getting the controller

let playbackController: AnimationPlaybackController

The animation playback controller managing the animation that triggered the event.

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Recognizing animation events

struct PlaybackStarted

The event raised when an animation has been started.

struct PlaybackLooped

The event raised when an animation loops.

struct PlaybackTerminated

The event raised when an animation has been terminated, regardless of whether it ran to completion.

