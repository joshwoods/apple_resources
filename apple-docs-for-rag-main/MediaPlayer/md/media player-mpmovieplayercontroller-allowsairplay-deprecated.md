

- Media Player
- MPMoviePlayerController
-  allowsAirPlay Deprecated

Instance Property

# allowsAirPlay

Specifies whether the movie player allows AirPlay movie playback.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var allowsAirPlay: Bool { get set }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

A movie player supports wireless movie playback to AirPlay-enabled hardware. When enabled, the user can select AirPlay-enabled hardware in the Control Panel when such hardware is in range.

The default value is true. To disable AirPlay movie playback, set this property’s value to false.

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

