

- UIKit
- UIFontPickerViewController
- UIFontPickerViewController.Configuration
-  filteredLanguagesPredicate Deprecated

Instance Property

# filteredLanguagesPredicate

A predicate to filter fonts based on the languages they support.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
@NSCopying @MainActor
var filteredLanguagesPredicate: NSPredicate? { get set }
```

## Discussion

By default, the font picker shows all available fonts, regardless of the languages they support. You may prefer to offer only fonts that support certain languages. To restrict the list, set this property to an NSPredicate defining the logic the font picker should apply to the fonts’ supported languages metadata.

Use language specifiers in the same format doc://com.apple.documentation/documentation/corefoundation/cflocale-rsj uses to specify languages in a filter predicate. You can use filterPredicate(forFilteredLanguages:) to construct a simple predicate that excludes fonts which don’t support any of a collection of languages you specify.

## See Also

### Filtering available fonts

var includeFaces: Bool

A Boolean value that determines whether the font picker should allow the user to select from font faces, or just font families.

var filteredTraits: UIFontDescriptor.SymbolicTraits

A predicate to filter fonts based on their traits, like bold, italic, or monospace.

class func filterPredicate(forFilteredLanguages: [String]) -> NSPredicate?

Creates a font picker filter based on language support.

Deprecated

