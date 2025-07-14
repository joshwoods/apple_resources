

- AVFoundation
-  AVPlaybackCoordinatorPlaybackControlDelegate 

Protocol

# AVPlaybackCoordinatorPlaybackControlDelegate

A protocol that defines the method to implement to respond to playback commands from the playback coordinator.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
protocol AVPlaybackCoordinatorPlaybackControlDelegate : NSObjectProtocol, Sendable
```

## Topics

### Responding to Commands

func playbackCoordinator(AVDelegatingPlaybackCoordinator, didIssue: AVDelegatingPlaybackCoordinatorPlayCommand, completionHandler: () -> Void)

Tells the delegate to match the playback rate to that of the group when the rate is nonzero.

**Required**

func playbackCoordinator(AVDelegatingPlaybackCoordinator, didIssue: AVDelegatingPlaybackCoordinatorPauseCommand, completionHandler: () -> Void)

Tells the delegate to pause playback.

**Required**

func playbackCoordinator(AVDelegatingPlaybackCoordinator, didIssue: AVDelegatingPlaybackCoordinatorSeekCommand, completionHandler: () -> Void)

Tells the delegate to seek to a new time.

**Required**

func playbackCoordinator(AVDelegatingPlaybackCoordinator, didIssue: AVDelegatingPlaybackCoordinatorBufferingCommand, completionHandler: () -> Void)

Tells the delegate to expect playback soon and to start buffering media data in preparation.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Creating a Coordinator

init(playbackControlDelegate: any AVPlaybackCoordinatorPlaybackControlDelegate)

Creates a playback coordinator for a custom playback object.

