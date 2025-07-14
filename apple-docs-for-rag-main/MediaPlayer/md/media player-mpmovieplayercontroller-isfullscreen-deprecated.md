

- Media Player
- MPMoviePlayerController
-  isFullscreen Deprecated

Instance Property

# isFullscreen

A Boolean that indicates whether the movie player is in full-screen mode.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isFullscreen: Bool { get set }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

The default value of this property is false. Changing the value of this property causes the movie player to enter or exit full-screen mode immediately. If you want to animate the transition to full-screen mode, use the setFullscreen(_:animated:) method instead.

Whenever the movie player enters or exits full-screen mode, it posts appropriate notifications to reflect the change. For example, upon entering full-screen mode, it posts MPMoviePlayerWillEnterFullscreenNotification and MPMoviePlayerDidEnterFullscreenNotification notifications. Upon exiting from full-screen mode, it posts MPMoviePlayerWillExitFullscreenNotification and MPMoviePlayerDidExitFullscreenNotification notifications.

The value of this property may also change as a result of the user interacting with the movie player controls.

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

