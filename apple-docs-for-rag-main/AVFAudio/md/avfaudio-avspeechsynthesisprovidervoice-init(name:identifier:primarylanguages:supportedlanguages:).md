

- AVFAudio
- AVSpeechSynthesisProviderVoice
-  init(name:identifier:primaryLanguages:supportedLanguages:) 

Initializer

# init(name:identifier:primaryLanguages:supportedLanguages:)

Creates a voice with a name, an identifier, and language information.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    name: String,
    identifier: String,
    primaryLanguages: [String],
    supportedLanguages: [String]
)
```

## Parameters 

`name`  

The localized name of the voice.

`identifier`  

The unique identifier for the voice.

`primaryLanguages`  

A list of BCP 47 codes that identify the primary languages.

`supportedLanguages`  

A list of BCP 47 codes that identify the languages the voice supports.

