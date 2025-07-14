

- WebKit
- WKWebViewConfiguration
-  allowsPictureInPictureMediaPlayback 

Instance Property

# allowsPictureInPictureMediaPlayback

A Boolean value that indicates whether HTML5 videos can play Picture in Picture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsPictureInPictureMediaPlayback: Bool { get set }
```

## Discussion

The default value of this property is true.

## See Also

### Setting media playback preferences

var allowsInlineMediaPlayback: Bool

A Boolean value that indicates whether HTML5 videos play inline or use the native full-screen controller.

var allowsAirPlayForMediaPlayback: Bool

A Boolean value that indicates whether the web view allows media playback over AirPlay.

var mediaTypesRequiringUserActionForPlayback: WKAudiovisualMediaTypes

The media types that require a user gesture to begin playing.

struct WKAudiovisualMediaTypes

The media types that require a user gesture to begin playing.

