

- Media Player
- MPNowPlayingInfoLanguageOptionGroup
-  init(languageOptions:defaultLanguageOption:allowEmptySelection:) 

Initializer

# init(languageOptions:defaultLanguageOption:allowEmptySelection:)

Creates a new language option group with the supplied language options.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
init(
    languageOptions: [MPNowPlayingInfoLanguageOption],
    defaultLanguageOption: MPNowPlayingInfoLanguageOption?,
    allowEmptySelection: Bool
)
```

## Parameters 

`languageOptions`  

An array containing the language options to associate with the language option group.

`defaultLanguageOption`  

The default language option for the group. Set this parameter to nil to denote there’s no default language option.

`allowEmptySelection`  

A Boolean that indicates whether the system requires a selection for the language option group.

## Return Value

A newly created language option group with the passed attributes.

