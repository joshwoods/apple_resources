

- AppKit
- NSText
-  isEditable 

Instance Property

# isEditable

A Boolean that controls whether the receiver allows the user to edit its text.

macOS

``` source
@MainActor
var isEditable: Bool { get set }
```

## Discussion

If `flag` is true, the receiver allows the user to edit text and attributes; if `flag` is false, it doesn’t.

You can change the receiver’s text programmatically regardless of this setting. If the receiver is made editable, it’s also made selectable. `NSText` objects are by default editable.

## See Also

### Setting behavioral attributes

var isSelectable: Bool

A Boolean that controls whether the receiver allows the user to select its text.

var isFieldEditor: Bool

A Boolean that controls whether the receiver interprets Tab, Shift-Tab, and Return (Enter) as cues to end editing and possibly to change the first responder.

var isRichText: Bool

A Boolean that controls whether the receiver allows the user to apply attributes to specific ranges of the text.

var importsGraphics: Bool

A Boolean that controls whether the receiver allows the user to import files by dragging.

