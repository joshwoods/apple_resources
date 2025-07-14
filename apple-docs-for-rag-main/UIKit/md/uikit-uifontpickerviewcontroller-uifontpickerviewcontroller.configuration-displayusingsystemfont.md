

- UIKit
- UIFontPickerViewController
- UIFontPickerViewController.Configuration
-  displayUsingSystemFont 

Instance Property

# displayUsingSystemFont

A Boolean value that determines whether to use the system font for all font names in the font picker.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var displayUsingSystemFont: Bool { get set }
```

## Discussion

By default, the font picker uses each font face to display that font face name in the font picker. Set this property to true if you want the font picker to display all font names in the system font instead.

