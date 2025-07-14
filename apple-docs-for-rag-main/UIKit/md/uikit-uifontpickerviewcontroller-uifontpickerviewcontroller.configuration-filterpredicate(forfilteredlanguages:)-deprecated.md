

- UIKit
- UIFontPickerViewController
- UIFontPickerViewController.Configuration
-  filterPredicate(forFilteredLanguages:) Deprecated

Type Method

# filterPredicate(forFilteredLanguages:)

Creates a font picker filter based on language support.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
@MainActor
class func filterPredicate(forFilteredLanguages filteredLanguages: [String]) -> NSPredicate?
```

## Parameters 

`filteredLanguages`  

Identifiers for the languages the font picker should include.

## Return Value

A predicate that is true when at least one of the provided strings is present.

## Discussion

Use this method to construct a predicate for filteredLanguagesPredicate that restricts the font picker’s list to only include fonts that support the filtered languages. Provide language identifiers in the same format doc://com.apple.documentation/documentation/corefoundation/cflocale-rsj uses.

## See Also

### Filtering available fonts

var includeFaces: Bool

A Boolean value that determines whether the font picker should allow the user to select from font faces, or just font families.

var filteredTraits: UIFontDescriptor.SymbolicTraits

A predicate to filter fonts based on their traits, like bold, italic, or monospace.

var filteredLanguagesPredicate: NSPredicate?

A predicate to filter fonts based on the languages they support.

Deprecated

