

- UIKit
- UIWebView
-  allowsPictureInPictureMediaPlayback Deprecated

Instance Property

# allowsPictureInPictureMediaPlayback

A Boolean value that determines whether Picture in Picture playback is allowed from this view.

iOS 9.0–12.0DeprecatediPadOS 9.0–12.0Deprecated

``` source
@MainActor
var allowsPictureInPictureMediaPlayback: Bool { get set }
```

## Discussion

The default value is true on devices that support Picture in Picture (PiP) mode and false on all other devices.

## See Also

### Managing media playback

var allowsInlineMediaPlayback: Bool

A Boolean value that determines whether HTML5 videos play inline or use the native full-screen controller.

Deprecated

var mediaPlaybackRequiresUserAction: Bool

A Boolean value that determines whether HTML5 videos can play automatically or require the user to start playing them.

Deprecated

var mediaPlaybackAllowsAirPlay: Bool

A Boolean value that determines whether Air Play is allowed from this view.

Deprecated

