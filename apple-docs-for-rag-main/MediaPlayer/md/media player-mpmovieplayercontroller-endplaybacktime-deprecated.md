

- Media Player
- MPMoviePlayerController
-  endPlaybackTime Deprecated

Instance Property

# endPlaybackTime

The end time (measured in seconds) for playback of the movie.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var endPlaybackTime: TimeInterval { get set }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

The default value of this property is -1, which indicates the natural end time of the movie. This property is not applicable for streamed content.

## See Also

### Controlling and monitoring playback

var loadState: MPMovieLoadState

The network load state of the movie player.

Deprecated

var playbackState: MPMoviePlaybackState

The current playback state of the movie player.

Deprecated

var initialPlaybackTime: TimeInterval

The time, specified in seconds within the video timeline, when playback should start.

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

