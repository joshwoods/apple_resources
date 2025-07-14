

- UIKit
- UIFontPickerViewController
- UIFontPickerViewController.Configuration
-  filteredTraits 

Instance Property

# filteredTraits

A predicate to filter fonts based on their traits, like bold, italic, or monospace.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var filteredTraits: UIFontDescriptor.SymbolicTraits { get set }
```

## See Also

### Filtering available fonts

var includeFaces: Bool

A Boolean value that determines whether the font picker should allow the user to select from font faces, or just font families.

var filteredLanguagesPredicate: NSPredicate?

A predicate to filter fonts based on the languages they support.

Deprecated

class func filterPredicate(forFilteredLanguages: [String]) -> NSPredicate?

Creates a font picker filter based on language support.

Deprecated

