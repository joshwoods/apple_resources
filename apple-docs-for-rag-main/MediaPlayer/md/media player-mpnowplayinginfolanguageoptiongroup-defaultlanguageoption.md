

- Media Player
- MPNowPlayingInfoLanguageOptionGroup
-  defaultLanguageOption 

Instance Property

# defaultLanguageOption

The default language option for the group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
var defaultLanguageOption: MPNowPlayingInfoLanguageOption? { get }
```

## Discussion

The value of this property is nil when there’s no default language option.

## See Also

### Retrieving language option group information

var allowEmptySelection: Bool

A Boolean that indicates whether the system requires a selection for the language option group.

var languageOptions: [MPNowPlayingInfoLanguageOption]

The available language options for the group.

