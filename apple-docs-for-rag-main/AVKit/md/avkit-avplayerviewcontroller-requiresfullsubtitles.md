

- AVKit
- AVPlayerViewController
-  requiresFullSubtitles 

Instance Property

# requiresFullSubtitles

A Boolean value that indicates whether the user can disable the display of subtitles.

tvOS 9.0+

``` source
@MainActor
var requiresFullSubtitles: Bool { get set }
```

## Discussion

When this property value is true, the subtitle menu doesn’t present the Off or Auto options, because subtitles are always displayed, if available.

The default value is false.

## See Also

### Managing Subtitles

var allowedSubtitleOptionLanguages: [String]?

An array of language codes that restrict the set of subtitle languages available to the user.

