

- UIKit
- UIFontPickerViewController
-  UIFontPickerViewController.Configuration 

Class

# UIFontPickerViewController.Configuration

The filters and display settings a font picker view controller uses to set up a font picker.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class Configuration
```

## Topics

### Customizing the font picker’s appearance

var displayUsingSystemFont: Bool

A Boolean value that determines whether to use the system font for all font names in the font picker.

### Filtering available fonts

var includeFaces: Bool

A Boolean value that determines whether the font picker should allow the user to select from font faces, or just font families.

var filteredTraits: UIFontDescriptor.SymbolicTraits

A predicate to filter fonts based on their traits, like bold, italic, or monospace.

var filteredLanguagesPredicate: NSPredicate?

A predicate to filter fonts based on the languages they support.

Deprecated

class func filterPredicate(forFilteredLanguages: [String]) -> NSPredicate?

Creates a font picker filter based on language support.

Deprecated

### Instance Properties

var languageFilter: Predicate&lt;[String]>?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Font picker

class UIFontPickerViewController

A view controller that manages the interface for selecting a font that the system provides or the user installs.

protocol UIFontPickerViewControllerDelegate

A set of optional methods for receiving messages about the user’s interaction with the font picker.

