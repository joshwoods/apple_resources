

- AppKit
- NSSpellChecker
-  availableLanguages 

Instance Property

# availableLanguages

Provides a list of all available languages.

macOS 10.5+

``` source
var availableLanguages: [String] { get }
```

## Return Value

An array containing all the available spell checking languages. The languages are ordered in the user’s preferred order as set in the system preferences.

## Discussion

If automaticallyIdentifiesLanguages is true, then text checking will automatically use this method as appropriate; otherwise, it will use the language set by setLanguage(_:).

The older checkSpelling(of:startingAt:language:wrap:inSpellDocumentWithTag:wordCount:) and checkGrammar(of:startingAt:language:wrap:inSpellDocumentWithTag:details:). methods will use the language set by setLanguage(_:), if they are called with a `nil` language argument.

## See Also

### Configuring Spell Checkers Languages

var userPreferredLanguages: [String]

Provides a subset of the available languages to be used for spell checking.

var automaticallyIdentifiesLanguages: Bool

Sets whether the spell checker will automatically identify languages.

func language() -> String

Returns the current language used in spell checking.

func setLanguage(String) -> Bool

Returns whether the specified language is in the Spelling pop-up list.

