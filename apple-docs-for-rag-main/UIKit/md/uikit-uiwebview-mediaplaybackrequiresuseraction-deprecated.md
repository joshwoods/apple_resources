

- UIKit
- UIWebView
-  mediaPlaybackRequiresUserAction Deprecated

Instance Property

# mediaPlaybackRequiresUserAction

A Boolean value that determines whether HTML5 videos can play automatically or require the user to start playing them.

iOS 4.0–12.0DeprecatediPadOS 4.0–12.0Deprecated

``` source
@MainActor
var mediaPlaybackRequiresUserAction: Bool { get set }
```

## Discussion

The default value on both iPad and iPhone is true. To make media play automatically when loaded, set this property to false and ensure the `` or `` element you want to play has the `autoplay` attribute set.

## See Also

### Managing media playback

var allowsInlineMediaPlayback: Bool

A Boolean value that determines whether HTML5 videos play inline or use the native full-screen controller.

Deprecated

var mediaPlaybackAllowsAirPlay: Bool

A Boolean value that determines whether Air Play is allowed from this view.

Deprecated

var allowsPictureInPictureMediaPlayback: Bool

A Boolean value that determines whether Picture in Picture playback is allowed from this view.

Deprecated

