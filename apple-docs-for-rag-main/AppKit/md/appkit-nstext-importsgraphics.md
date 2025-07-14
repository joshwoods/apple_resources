

- AppKit
- NSText
-  importsGraphics 

Instance Property

# importsGraphics

A Boolean that controls whether the receiver allows the user to import files by dragging.

macOS

``` source
@MainActor
var importsGraphics: Bool { get set }
```

## Discussion

If `flag` is true, the receiver allows the user to import files by dragging; if `flag` is false, it doesn’t.

If the receiver is set to accept dragged files, it’s also made a rich text object. Subclasses may or may not accept dragged files by default.

## See Also

### Setting behavioral attributes

var isEditable: Bool

A Boolean that controls whether the receiver allows the user to edit its text.

var isSelectable: Bool

A Boolean that controls whether the receiver allows the user to select its text.

var isFieldEditor: Bool

A Boolean that controls whether the receiver interprets Tab, Shift-Tab, and Return (Enter) as cues to end editing and possibly to change the first responder.

var isRichText: Bool

A Boolean that controls whether the receiver allows the user to apply attributes to specific ranges of the text.

