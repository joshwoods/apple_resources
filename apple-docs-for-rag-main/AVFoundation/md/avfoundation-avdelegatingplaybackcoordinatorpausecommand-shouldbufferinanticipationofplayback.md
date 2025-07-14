

- AVFoundation
- AVDelegatingPlaybackCoordinatorPauseCommand
-  shouldBufferInAnticipationOfPlayback 

Instance Property

# shouldBufferInAnticipationOfPlayback

A Boolean value that indicates whether the player starts buffering in preparation for a request to begin playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var shouldBufferInAnticipationOfPlayback: Bool { get }
```

## Discussion

A true value indicates that a participant player requests starting playback at the anticipatedPlaybackRate value.

## See Also

### Accessing Command Details

var anticipatedPlaybackRate: Float

The rate at which the coordinator expects the current item to play.

