

- AVFoundation
- AVMutableMovieTrack
-  languageCode 

Instance Property

# languageCode

The language code of the track.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var languageCode: String? { get set }
```

## Discussion

The value is an ISO 639-2/T language code, or `nil` if the track doesn’t specify a language code.

## See Also

### Accessing Language Support

var extendedLanguageTag: String?

The language tag of the track.

