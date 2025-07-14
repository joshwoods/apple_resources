

- Media Player
- MPMoviePlayerController
-  playbackState Deprecated

Instance Property

# playbackState

The current playback state of the movie player.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var playbackState: MPMoviePlaybackState { get }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

The playback state is affected by programmatic calls to play, pause, or stop the movie player. It can also be affected by user interactions or by the network, in cases where streaming content cannot be buffered fast enough.

See the MPMoviePlaybackState enumeration for possible values of this property. To be notified of changes to the playback state of a movie player, register for the MPMoviePlayerPlaybackStateDidChangeNotification notification.

## See Also

### Controlling and monitoring playback

var loadState: MPMovieLoadState

The network load state of the movie player.

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

var timedMetadata: [Any]!

Obtains the most recent time-based metadata provided by the streamed movie.

Deprecated

