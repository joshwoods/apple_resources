

- AppKit
- NSFontManager
-  sendAction() 

Instance Method

# sendAction()

A Boolean value that indicates whether a responder handled the font manager’s action message.

macOS

``` source
func sendAction() -> Bool
```

## Discussion

By default, the font manager’s action message is changeFont:. The value of this property is true if some responder object handled the changeFont: message or false if the message went unheard.

## See Also

### Related Documentation

var action: Selector

The action sent to the first responder when the user selects a new font from the Font panel or chooses a command from the Font menu.

### Setting and Examining the Selected Font

func setSelectedFont(NSFont, isMultiple: Bool)

Records the specified font as the currently selected font and updates the Font panel.

var selectedFont: NSFont?

The currently selected font object.

var isMultiple: Bool

A Boolean value that indicates whether the currently selected font has multiple fonts.

func localizedName(forFamily: String, face: String?) -> String

Returns a localized string with the name of the specified font family and face, if one exists.

