

- Media Player
- MPMoviePlayerController
-  readyForDisplay Deprecated

Instance Property

# readyForDisplay

A Boolean that indicates whether the first video frame of the movie is ready to be displayed.

iOS 6.0–9.0DeprecatediPadOS 6.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var readyForDisplay: Bool { get }
```

## Discussion

The default value of this property is false. This property returns true if the first video frame is ready to be displayed and returns false if there are no video tracks associated. When the value of this property changes to true, a MPMoviePlayerReadyForDisplayDidChangeNotification is sent.

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

var repeatMode: MPMovieRepeatMode

Determines how the movie player repeats the playback of the movie.

Deprecated

var timedMetadata: [Any]!

Obtains the most recent time-based metadata provided by the streamed movie.

Deprecated

