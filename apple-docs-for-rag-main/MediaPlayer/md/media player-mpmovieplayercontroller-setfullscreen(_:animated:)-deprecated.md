

- Media Player
- MPMoviePlayerController
-  setFullscreen(\_:animated:) Deprecated

Instance Method

# setFullscreen(\_:animated:)

Causes the movie player to enter or exit full-screen mode.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func setFullscreen(
    _ fullscreen: Bool,
    animated: Bool
)
```

Deprecated

Use AVPlayerViewController in AVKit

## Parameters 

`fullscreen`  

Specify true to enter full-screen mode or false to exit full-screen mode.

`animated`  

Specify true to animate the transition between modes or false to switch immediately to the new mode.

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

var scalingMode: MPMovieScalingMode

The scaling mode to use when displaying the movie.

Deprecated

var controlStyle: MPMovieControlStyle

The style of the playback controls.

Deprecated

var useApplicationAudioSession: Bool

A Boolean value that indicates whether the movie player should use the app’s audio session.

Deprecated

