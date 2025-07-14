

- Translation
- TranslationSession
- TranslationSession.Configuration
-  init(source:target:) 

Initializer

# init(source:target:)

Creates a configuration from a source and target language.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
init(
    source: Locale.Language? = nil,
    target: Locale.Language? = nil
)
```

## Parameters 

`source`  

The language the source content is in. If `nil` the session tries to identify the language, and prompt the user to pick the source language if it’s unclear. All text translated with this session should be in the same source language.

`target`  

The language to translate content into. If `nil` the session tries to pick a target language according to the user’s `Locale/preferredLanguages`, and the `source`.

## Discussion

When creating a translation session configuration it’s best to use `Locale.Language` values that return from supportedLanguages. When you pass other `Locale.Language` values the framework tries to match to one of these supported languages.

