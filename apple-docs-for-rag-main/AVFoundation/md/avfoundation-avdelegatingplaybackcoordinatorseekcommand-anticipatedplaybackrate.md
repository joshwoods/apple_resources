

- AVFoundation
- AVDelegatingPlaybackCoordinatorSeekCommand
-  anticipatedPlaybackRate 

Instance Property

# anticipatedPlaybackRate

The rate at which the coordinator expects playback to resume.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var anticipatedPlaybackRate: Float { get }
```

## See Also

### Accessing Command Details

var shouldBufferInAnticipationOfPlayback: Bool

A Boolean value that indicates whether the player starts buffering in anticipation of a request to begin playback.

var itemTime: CMTime

The time to seek to in the item timeline.

var completionDueDate: Date?

The deadline by which the coordinator expects the delegate to handle the command.

