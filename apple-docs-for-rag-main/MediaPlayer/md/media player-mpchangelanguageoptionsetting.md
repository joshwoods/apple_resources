

- Media Player
-  MPChangeLanguageOptionSetting 

Enumeration

# MPChangeLanguageOptionSetting

The states that determine when language option changes take effect.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.2+visionOS 1.0+watchOS 5.0+

``` source
enum MPChangeLanguageOptionSetting
```

## Topics

### Enumeration Cases

case none

No language option change is to be made.

case nowPlayingItemOnly

The language option change is applied to the now playing item only.

case permanent

The language option change is applied to all future playback items.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Changing the language option

var languageOption: MPNowPlayingInfoLanguageOption

The requested language option to change.

var setting: MPChangeLanguageOptionSetting

The extent of the language setting change.

