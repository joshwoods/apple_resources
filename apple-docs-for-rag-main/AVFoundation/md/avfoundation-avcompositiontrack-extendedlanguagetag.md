

- AVFoundation
- AVCompositionTrack
-  extendedLanguageTag 

Instance Property

# extendedLanguageTag

The language tag of the track.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var extendedLanguageTag: String? { get }
```

## Discussion

The value is a BCP-47 language tag, or `nil` if the track doesn’t specify a language tag.

## See Also

### Accessing Language Support

var languageCode: String?

The language code of the track.

