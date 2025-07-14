

- Media Player
- MPMoviePlayerController
-  initialPlaybackTime Deprecated

Instance Property

# initialPlaybackTime

The time, specified in seconds within the video timeline, when playback should start.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var initialPlaybackTime: TimeInterval { get set }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

For progressively downloaded content, playback starts at the closest key frame prior to the provided time. For video-on-demand content, playback starts at the nearest segment boundary to the provided time. For live video streams, the playback start time is measured from the start of the current playlist and is rounded to the nearest segment boundary.

The default value of this property is -1, which indicates the natural start time of the movie.

## See Also

### Controlling and monitoring playback

var loadState: MPMovieLoadState

The network load state of the movie player.

Deprecated

var playbackState: MPMoviePlaybackState

The current playback state of the movie player.

Deprecated

var endPlaybackTime: TimeInterval

The end time (measured in seconds) for playback of the movie.

Deprecated

var shouldAutoplay: Bool

A Boolean that indicates whether a movie should begin playback automatically.

Deprecated

var readyForDisplay: Bool

A Boolean that indicates whether the first video frame of the movie is ready to be displayed.

Deprecated

var repeatMode: MPMovieRepeatMode

Determines how the movie player repeats the playback of the movie.

Deprecated

var timedMetadata: [Any]!

Obtains the most recent time-based metadata provided by the streamed movie.

Deprecated

