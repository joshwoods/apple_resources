

- UIKit
- UIFontPickerViewController
- UIFontPickerViewController.Configuration
-  includeFaces 

Instance Property

# includeFaces

A Boolean value that determines whether the font picker should allow the user to select from font faces, or just font families.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var includeFaces: Bool { get set }
```

## Discussion

By default, the font picker only lists font families, like Times New Roman or Helvetica. Set includeFaces to true so the user can select a specific font face, such as Times New Roman Bold or Helvetica Light Oblique.

## See Also

### Filtering available fonts

var filteredTraits: UIFontDescriptor.SymbolicTraits

A predicate to filter fonts based on their traits, like bold, italic, or monospace.

var filteredLanguagesPredicate: NSPredicate?

A predicate to filter fonts based on the languages they support.

Deprecated

class func filterPredicate(forFilteredLanguages: [String]) -> NSPredicate?

Creates a font picker filter based on language support.

Deprecated

