

- AVFoundation
- AVPlaybackCoordinatorPlaybackControlDelegate
-  playbackCoordinator(\_:didIssue:completionHandler:) 

Instance Method

# playbackCoordinator(\_:didIssue:completionHandler:)

Tells the delegate to expect playback soon and to start buffering media data in preparation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func playbackCoordinator(
    _ coordinator: AVDelegatingPlaybackCoordinator,
    didIssue bufferingCommand: AVDelegatingPlaybackCoordinatorBufferingCommand,
    completionHandler: @escaping () -> Void
)
```

``` source
func playbackCoordinator(
    _ coordinator: AVDelegatingPlaybackCoordinator,
    didIssue bufferingCommand: AVDelegatingPlaybackCoordinatorBufferingCommand
) async
```

**Required**

## Parameters 

`coordinator`  

The playback coordinator that issues the command.

`bufferingCommand`  

The command to execute. Before performing it, verify that its expectedCurrentItemIdentifier property value matches the item that you’re currently playing. If the command isn’t valid for the current item, ignore it and call the completion handler.

`completionHandler`  

A completion handler that your app must call when it finishes handling the command, either successfully or after beginning a suspension if it can’t handle the command currently.

If the value of the command’s shouldBufferInAnticipationOfPlayback property is true, call the completion handler only after the player is ready for playback.

## Discussion

The coordinator issues this command when playback is currently in a paused state and the coordinator is expecting playback to start soon. It provides an appropriate opportunity to update your player UI to indicate that playback is in a waiting state.

## See Also

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

