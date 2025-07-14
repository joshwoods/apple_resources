

- AppKit
- NSSpellChecker
-  automaticallyIdentifiesLanguages 

Instance Property

# automaticallyIdentifiesLanguages

Sets whether the spell checker will automatically identify languages.

macOS 10.6+

``` source
var automaticallyIdentifiesLanguages: Bool { get set }
```

## Parameters 

`flag`  

true if languages should be automatically identified, otherwise false.

## See Also

### Configuring Spell Checkers Languages

var availableLanguages: [String]

Provides a list of all available languages.

var userPreferredLanguages: [String]

Provides a subset of the available languages to be used for spell checking.

func language() -> String

Returns the current language used in spell checking.

func setLanguage(String) -> Bool

Returns whether the specified language is in the Spelling pop-up list.

