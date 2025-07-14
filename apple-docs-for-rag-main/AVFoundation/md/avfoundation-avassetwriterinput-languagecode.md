

- AVFoundation
- AVAssetWriterInput
-  languageCode 

Instance Property

# languageCode

The language code of the input’s track.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var languageCode: String? { get set }
```

## Discussion

Specify an ISO 639-2/T language code value, or `nil` to prevent the writer from writing a language code.

## See Also

### Configuring Language Support

var extendedLanguageTag: String?

The extended language for the input’s track.

