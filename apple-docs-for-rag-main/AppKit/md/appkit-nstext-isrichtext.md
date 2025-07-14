

- AppKit
- NSText
-  isRichText 

Instance Property

# isRichText

A Boolean that controls whether the receiver allows the user to apply attributes to specific ranges of the text.

macOS

``` source
@MainActor
var isRichText: Bool { get set }
```

## Discussion

If `flag` is true the receiver allows the user to apply attributes to specific ranges of the text; if `flag` is false it doesn’t.

## See Also

### Setting behavioral attributes

var isEditable: Bool

A Boolean that controls whether the receiver allows the user to edit its text.

var isSelectable: Bool

A Boolean that controls whether the receiver allows the user to select its text.

var isFieldEditor: Bool

A Boolean that controls whether the receiver interprets Tab, Shift-Tab, and Return (Enter) as cues to end editing and possibly to change the first responder.

var importsGraphics: Bool

A Boolean that controls whether the receiver allows the user to import files by dragging.

