

- AVKit
- AVPlayerViewController
-  allowedSubtitleOptionLanguages 

Instance Property

# allowedSubtitleOptionLanguages

An array of language codes that restrict the set of subtitle languages available to the user.

tvOS 9.0+

``` source
@MainActor
var allowedSubtitleOptionLanguages: [String]? { get set }
```

## Discussion

When this property value is `nil` (the default), the player view controller UI presents all available subtitle options. The Auto subtitle option is only available when this property value is `nil` and requiresFullSubtitles is false.

To allow only a restricted subset of subtitles, set this property value to an array of BCP 47 language codes. Restricting the set of subtitle languages makes the Auto option unavailable.

## See Also

### Managing Subtitles

var requiresFullSubtitles: Bool

A Boolean value that indicates whether the user can disable the display of subtitles.

