

- Media Player
- MPMoviePlayerController
-  controlStyle Deprecated

Instance Property

# controlStyle

The style of the playback controls.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var controlStyle: MPMovieControlStyle { get set }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

The default value of this property is default. You can change the value of this property to change the style of the controls or to hide the controls altogether. For a list of available control styles, see MPMovieControlStyle.

## See Also

### Accessing movie properties

var contentURL: URL!

The URL that points to the movie file.

Deprecated

var movieSourceType: MPMovieSourceType

The playback type of the movie.

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

var useApplicationAudioSession: Bool

A Boolean value that indicates whether the movie player should use the app’s audio session.

Deprecated

