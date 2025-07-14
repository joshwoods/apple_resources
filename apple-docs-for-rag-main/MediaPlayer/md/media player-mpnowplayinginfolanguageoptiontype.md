

- Media Player
-  MPNowPlayingInfoLanguageOptionType 

Enumeration

# MPNowPlayingInfoLanguageOptionType

The language option type to use for the Now Playing item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
enum MPNowPlayingInfoLanguageOptionType
```

## Topics

### Enumeration Cases

case audible

Indicates an audible language option is used.

case legible

Indicates a written language option is used.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Retrieving language option properties

var displayName: String?

The display name for a language option.

var identifier: String?

The unique identifier for the language option.

var languageOptionCharacteristics: [String]?

The characteristics that describe the content of the language option.

var languageTag: String?

The abbreviated language code for the language option.

var languageOptionType: MPNowPlayingInfoLanguageOptionType

The type of language option.

