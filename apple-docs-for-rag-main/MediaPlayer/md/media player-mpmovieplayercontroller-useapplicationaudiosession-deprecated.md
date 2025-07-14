

- Media Player
- MPMoviePlayerController
-  useApplicationAudioSession Deprecated

Instance Property

# useApplicationAudioSession

A Boolean value that indicates whether the movie player should use the app’s audio session.

iOS 6.0–9.0DeprecatediPadOS 6.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var useApplicationAudioSession: Bool { get set }
```

Deprecated

There is not replacement for this property and its use is discouraged.

## Discussion

The default value of this property is true. Setting this property to false causes the movie player to use a system-supplied audio session with a non-mixable playback category.

When this property is true, the movie player shares the app’s audio session. This give you control over how the movie player content interacts with your audio and with audio from other apps, such as the iPod. For important guidance on using this feature, see Audio Session Programming Guide in Audio Session Programming Guide.

Changing the value of this property does not affect the currently playing movie. For the new setting to take effect, you must stop playback and then start it again.

### Special considerations

In iOS 3.1 and earlier, a movie player always uses a system-supplied audio session. To obtain that same behavior in iOS 3.2 and newer, you must set this property’s value to false.

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

var controlStyle: MPMovieControlStyle

The style of the playback controls.

Deprecated

