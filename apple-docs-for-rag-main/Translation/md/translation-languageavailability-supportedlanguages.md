

- Translation
- LanguageAvailability
-  supportedLanguages 

Instance Property

# supportedLanguages

A list of translation languages the framework supports.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
var supportedLanguages: [Locale.Language] { get async }
```

## Return Value

An array of languages the framework supports.

## Discussion

A language must download before it can be used in a translation.

