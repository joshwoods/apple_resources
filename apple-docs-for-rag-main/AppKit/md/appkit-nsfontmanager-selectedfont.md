

- AppKit
- NSFontManager
-  selectedFont 

Instance Property

# selectedFont

The currently selected font object.

macOS

``` source
var selectedFont: NSFont? { get }
```

## Discussion

The value of this property is the last font recorded with a setSelectedFont(_:isMultiple:) message.

While fonts are being converted in response to a convert(_:) message, you can determine the font selected in the Font panel like this:

```
NSFontManager *fontManager = [NSFontManager sharedFontManager];
panelFont = [fontManager convertFont:[fontManager.selectedFont]];
```

## See Also

### Setting and Examining the Selected Font

func setSelectedFont(NSFont, isMultiple: Bool)

Records the specified font as the currently selected font and updates the Font panel.

var isMultiple: Bool

A Boolean value that indicates whether the currently selected font has multiple fonts.

func sendAction() -> Bool

A Boolean value that indicates whether a responder handled the font manager’s action message.

func localizedName(forFamily: String, face: String?) -> String

Returns a localized string with the name of the specified font family and face, if one exists.

