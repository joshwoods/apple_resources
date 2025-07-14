

- Translation
- TranslationSession
- TranslationSession.Configuration
-  source 

Instance Property

# source

The language to translate content from.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
var source: Locale.Language?
```

## Discussion

If left to its default value of `nil`, the session tries to identify the source language automatically, and prompts the user to choose a source language if it’s unclear. Changing this value cancels the previous task and creates a new one.

