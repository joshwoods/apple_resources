

- AppKit
- NSText
-  isFieldEditor 

Instance Property

# isFieldEditor

A Boolean that controls whether the receiver interprets Tab, Shift-Tab, and Return (Enter) as cues to end editing and possibly to change the first responder.

macOS

``` source
@MainActor
var isFieldEditor: Bool { get set }
```

## Discussion

If `flag` is true, the receiver interprets Tab, Shift-Tab, and Return (Enter) as cues to end editing and possibly to change the first responder; if `flag` is false, it doesn’t, instead accepting these characters as text input.

See the NSWindow class specification for more information on field editors. By default, `NSText` objects don’t behave as field editors.

## See Also

### Setting behavioral attributes

var isEditable: Bool

A Boolean that controls whether the receiver allows the user to edit its text.

var isSelectable: Bool

A Boolean that controls whether the receiver allows the user to select its text.

var isRichText: Bool

A Boolean that controls whether the receiver allows the user to apply attributes to specific ranges of the text.

var importsGraphics: Bool

A Boolean that controls whether the receiver allows the user to import files by dragging.

