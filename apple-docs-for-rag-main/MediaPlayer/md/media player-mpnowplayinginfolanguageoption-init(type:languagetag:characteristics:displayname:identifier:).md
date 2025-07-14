

- Media Player
- MPNowPlayingInfoLanguageOption
-  init(type:languageTag:characteristics:displayName:identifier:) 

Initializer

# init(type:languageTag:characteristics:displayName:identifier:)

Creates a single language option.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
init(
    type languageOptionType: MPNowPlayingInfoLanguageOptionType,
    languageTag: String,
    characteristics languageOptionCharacteristics: [String]?,
    displayName: String,
    identifier: String
)
```

## Parameters 

`languageOptionType`  

The type, audio or legible, for the language option.

`languageTag`  

The IETF BCP 47 language tag for the language option.

`languageOptionCharacteristics`  

An array of characteristics that describes the language option.

`displayName`  

The name for displaying the language option.

`identifier`  

A unique identifier for the language option.

## Return Value

A newly created language option containing the passed characteristics.

