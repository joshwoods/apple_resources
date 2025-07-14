

- Translation
- TranslationSession
-  sourceLanguage 

Instance Property

# sourceLanguage

The input language to translate from.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
final let sourceLanguage: Locale.Language?
```

## Discussion

If this value is set to `nil` the session tries to identify the source language automatically. If it can’t, it prompts the user to choose the source language to use for the translation.

Note

This value doesn’t update after translation; to see what source language the session uses for a particular translation, check the response sourceLanguage.

## See Also

### Getting configuration

let targetLanguage: Locale.Language?

The output language to translate into.

