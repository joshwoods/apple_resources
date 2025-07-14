

- AVFoundation
- AVMutableMovieTrack
-  extendedLanguageTag 

Instance Property

# extendedLanguageTag

The language tag of the track.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var extendedLanguageTag: String? { get set }
```

## Discussion

The value is a BCP-47 language tag, or `nil` if the track doesn’t specify a language tag.

## See Also

### Accessing Language Support

var languageCode: String?

The language code of the track.

