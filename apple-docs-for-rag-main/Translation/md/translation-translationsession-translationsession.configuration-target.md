

- Translation
- TranslationSession
- TranslationSession.Configuration
-  target 

Instance Property

# target

The language to translate content into.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
var target: Locale.Language?
```

## Discussion

If left to its default value of `nil`, the session picks a target language according to the user’s `Locale/preferredLanguages`, and the `source`. Changing this value cancels the previous tasks and creates a new one.

