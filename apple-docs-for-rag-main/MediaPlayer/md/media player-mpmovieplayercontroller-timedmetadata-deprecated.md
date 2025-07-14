

- Media Player
- MPMoviePlayerController
-  timedMetadata Deprecated

Instance Property

# timedMetadata

Obtains the most recent time-based metadata provided by the streamed movie.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var timedMetadata: [Any]! { get }
```

Deprecated

Use AVPlayerViewController in AVKit.

## Return Value

An array of the most recent MPTimedMetadata objects provided by the streamed movie.

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

