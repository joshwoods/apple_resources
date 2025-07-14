

- Media Player
- MPMoviePlayerController
-  movieSourceType Deprecated

Instance Property

# movieSourceType

The playback type of the movie.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var movieSourceType: MPMovieSourceType { get set }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

The default value of this property is MPMovieSourceType.unknown. This property provides a clue to the playback system as to how it should download and buffer the movie content. If you know the source type of the movie, setting the value of this property before playback begins can improve the load times for the movie content. If you do not set the source type explicitly before playback, the movie player controller must gather this information, which might delay playback.

## See Also

### Accessing movie properties

var contentURL: URL!

The URL that points to the movie file.

Deprecated

var movieMediaTypes: MPMovieMediaTypeMask

The types of media available in the movie.

Deprecated

var allowsAirPlay: Bool

Specifies whether the movie player allows AirPlay movie playback.

Deprecated

var isAirPlayVideoActive: Bool

Indicates whether the movie player is currently playing video via AirPlay.

Deprecated

var naturalSize: CGSize

The width and height of the movie frame.

Deprecated

var isFullscreen: Bool

A Boolean that indicates whether the movie player is in full-screen mode.

Deprecated

func setFullscreen(Bool, animated: Bool)

Causes the movie player to enter or exit full-screen mode.

Deprecated

var scalingMode: MPMovieScalingMode

The scaling mode to use when displaying the movie.

Deprecated

var controlStyle: MPMovieControlStyle

The style of the playback controls.

Deprecated

var useApplicationAudioSession: Bool

A Boolean value that indicates whether the movie player should use the app’s audio session.

Deprecated

