

- AppKit
- NSFontManager
-  isMultiple 

Instance Property

# isMultiple

A Boolean value that indicates whether the currently selected font has multiple fonts.

macOS

``` source
var isMultiple: Bool { get }
```

## Discussion

When the value of this property is true, the last font selection recorded has multiple fonts; if the last font selection recorded is a single font, the value is false.

## See Also

### Setting and Examining the Selected Font

func setSelectedFont(NSFont, isMultiple: Bool)

Records the specified font as the currently selected font and updates the Font panel.

var selectedFont: NSFont?

The currently selected font object.

func sendAction() -> Bool

A Boolean value that indicates whether a responder handled the font manager’s action message.

func localizedName(forFamily: String, face: String?) -> String

Returns a localized string with the name of the specified font family and face, if one exists.

