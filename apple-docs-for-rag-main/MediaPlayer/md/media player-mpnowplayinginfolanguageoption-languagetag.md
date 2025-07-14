

- Media Player
- MPNowPlayingInfoLanguageOption
-  languageTag 

Instance Property

# languageTag

The abbreviated language code for the language option.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
var languageTag: String? { get }
```

## Discussion

This property contains the IETF BCP 47 language code for the language option. A value of nil indicates that this option is disabled.

## See Also

### Retrieving language option properties

var displayName: String?

The display name for a language option.

var identifier: String?

The unique identifier for the language option.

var languageOptionCharacteristics: [String]?

The characteristics that describe the content of the language option.

var languageOptionType: MPNowPlayingInfoLanguageOptionType

The type of language option.

enum MPNowPlayingInfoLanguageOptionType

The language option type to use for the Now Playing item.

