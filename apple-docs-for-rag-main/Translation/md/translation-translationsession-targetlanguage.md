

- Translation
- TranslationSession
-  targetLanguage 

Instance Property

# targetLanguage

The output language to translate into.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
final let targetLanguage: Locale.Language?
```

## Discussion

If this value is set to `nil` the session chooses an optimal language to translate into based on the `sourceLanguage`, and the user’s `Locale/preferredLanguages`.

Note

This value doesn’t update after translation; to see what target language the session uses for a particular translation, check the response targetLanguage.

## See Also

### Getting configuration

let sourceLanguage: Locale.Language?

The input language to translate from.

