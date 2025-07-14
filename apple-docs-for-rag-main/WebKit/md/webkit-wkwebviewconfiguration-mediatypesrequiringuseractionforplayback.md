

- WebKit
- WKWebViewConfiguration
-  mediaTypesRequiringUserActionForPlayback 

Instance Property

# mediaTypesRequiringUserActionForPlayback

The media types that require a user gesture to begin playing.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+

``` source
@MainActor
var mediaTypesRequiringUserActionForPlayback: WKAudiovisualMediaTypes { get set }
```

## Discussion

Use WKAudiovisualMediaTypeNone to indicate that no user gestures are required to begin playing media.

## See Also

### Setting media playback preferences

var allowsInlineMediaPlayback: Bool

A Boolean value that indicates whether HTML5 videos play inline or use the native full-screen controller.

var allowsAirPlayForMediaPlayback: Bool

A Boolean value that indicates whether the web view allows media playback over AirPlay.

var allowsPictureInPictureMediaPlayback: Bool

A Boolean value that indicates whether HTML5 videos can play Picture in Picture.

struct WKAudiovisualMediaTypes

The media types that require a user gesture to begin playing.

