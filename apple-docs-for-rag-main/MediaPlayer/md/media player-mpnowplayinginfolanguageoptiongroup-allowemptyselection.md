

- Media Player
- MPNowPlayingInfoLanguageOptionGroup
-  allowEmptySelection 

Instance Property

# allowEmptySelection

A Boolean that indicates whether the system requires a selection for the language option group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
var allowEmptySelection: Bool { get }
```

## Discussion

When set to true, there must be a language option in the language option group.

## See Also

### Retrieving language option group information

var defaultLanguageOption: MPNowPlayingInfoLanguageOption?

The default language option for the group.

var languageOptions: [MPNowPlayingInfoLanguageOption]

The available language options for the group.

