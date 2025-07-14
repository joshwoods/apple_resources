

- AppKit
- NSSpellChecker
-  userPreferredLanguages 

Instance Property

# userPreferredLanguages

Provides a subset of the available languages to be used for spell checking.

macOS 10.6+

``` source
var userPreferredLanguages: [String] { get }
```

## Return Value

An array containing the user’s preferred languages for spell checking. The order is set in the system preferences.

## Discussion

If automaticallyIdentifiesLanguages is true, then text checking will automatically use this method as appropriate; otherwise, it will use the language set by setLanguage(_:).

The older checkSpelling(of:startingAt:language:wrap:inSpellDocumentWithTag:wordCount:) and checkGrammar(of:startingAt:language:wrap:inSpellDocumentWithTag:details:). methods will use the language set by setLanguage(_:), if they are called with a `nil` language argument.

## See Also

### Configuring Spell Checkers Languages

var availableLanguages: [String]

Provides a list of all available languages.

var automaticallyIdentifiesLanguages: Bool

Sets whether the spell checker will automatically identify languages.

func language() -> String

Returns the current language used in spell checking.

func setLanguage(String) -> Bool

Returns whether the specified language is in the Spelling pop-up list.

