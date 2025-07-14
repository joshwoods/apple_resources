

- AppKit
- NSSpellChecker
-  language() 

Instance Method

# language()

Returns the current language used in spell checking.

macOS

``` source
func language() -> String
```

## Return Value

The current spell checking language, as a string.

## Discussion

The result string specifies the language using the language and regional designations described in Language and Locale Designations in Internationalization and Localization Guide.

## See Also

### Configuring Spell Checkers Languages

var availableLanguages: [String]

Provides a list of all available languages.

var userPreferredLanguages: [String]

Provides a subset of the available languages to be used for spell checking.

var automaticallyIdentifiesLanguages: Bool

Sets whether the spell checker will automatically identify languages.

func setLanguage(String) -> Bool

Returns whether the specified language is in the Spelling pop-up list.

