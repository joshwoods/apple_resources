

- WebKit
- WKWebViewConfiguration
-  allowsInlineMediaPlayback 

Instance Property

# allowsInlineMediaPlayback

A Boolean value that indicates whether HTML5 videos play inline or use the native full-screen controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsInlineMediaPlayback: Bool { get set }
```

## Discussion

Set this property to true to play videos inline, or false to use the native full-screen controller. When adding a video element to an HTML document on iPhone, you must also include the `playsinline` attribute.

The default value of this property is false for iPhone and true for iPad.

Important

Apps created before iOS 10.0 must use the `webkit-playsinline` attribute.

## See Also

### Setting media playback preferences

var allowsAirPlayForMediaPlayback: Bool

A Boolean value that indicates whether the web view allows media playback over AirPlay.

var allowsPictureInPictureMediaPlayback: Bool

A Boolean value that indicates whether HTML5 videos can play Picture in Picture.

var mediaTypesRequiringUserActionForPlayback: WKAudiovisualMediaTypes

The media types that require a user gesture to begin playing.

struct WKAudiovisualMediaTypes

The media types that require a user gesture to begin playing.

