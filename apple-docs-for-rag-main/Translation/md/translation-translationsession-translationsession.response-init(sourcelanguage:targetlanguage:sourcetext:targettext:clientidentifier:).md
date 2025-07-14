

- Translation
- TranslationSession
- TranslationSession.Response
-  init(sourceLanguage:targetLanguage:sourceText:targetText:clientIdentifier:) 

Initializer

# init(sourceLanguage:targetLanguage:sourceText:targetText:clientIdentifier:)

Creates an instance of a translation response.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
init(
    sourceLanguage: Locale.Language,
    targetLanguage: Locale.Language,
    sourceText: String,
    targetText: String,
    clientIdentifier: String? = nil
)
```

## Discussion

You don’t normally use this initializer directly. Instead, let the translation functions create instances of this type for you. Do use this initializer when you want to create sample response for a test, for example in a SwiftUI preview.

