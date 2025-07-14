

- AppKit
- NSText
-  isSelectable 

Instance Property

# isSelectable

A Boolean that controls whether the receiver allows the user to select its text.

macOS

``` source
@MainActor
var isSelectable: Bool { get set }
```

## Discussion

If `flag` is true, the receiver allows the user to select text; if `flag` is false, it doesn’t.

You can set selections programmatically regardless of this setting. If the receiver is made not selectable, it’s also made not editable. `NSText` objects are by default editable and selectable.

## See Also

### Setting behavioral attributes

var isEditable: Bool

A Boolean that controls whether the receiver allows the user to edit its text.

var isFieldEditor: Bool

A Boolean that controls whether the receiver interprets Tab, Shift-Tab, and Return (Enter) as cues to end editing and possibly to change the first responder.

var isRichText: Bool

A Boolean that controls whether the receiver allows the user to apply attributes to specific ranges of the text.

var importsGraphics: Bool

A Boolean that controls whether the receiver allows the user to import files by dragging.

