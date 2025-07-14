

- AppKit
- NSCell
-  sendsActionOnEndEditing 

Instance Property

# sendsActionOnEndEditing

A Boolean value indicating whether the cell’s control object sends its action message when the user finishes editing the cell’s text.

macOS

``` source
@MainActor
var sendsActionOnEndEditing: Bool { get set }
```

## Discussion

When the value of this property is true, the control sends its action message when editing is complete. Editing is complete when the user does one of the following:

- Presses the Return key

- Presses the Tab key to move out of the field

- Clicks another text field

When the value is false, the control sends its action message only when the user presses the Return key.

## See Also

### Editing and Selecting Text

func edit(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, event: NSEvent?)

Begins editing of the receiver’s text using the specified field editor.

func select(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the cell’s field editor.

func endEditing(NSText)

Ends the editing of text in the receiver using the specified field editor.

var wantsNotificationForMarkedText: Bool

A Boolean value indicating whether the cell’s field editor should post text change notifications.

func fieldEditor(for: NSView) -> NSTextView?

Returns a custom field editor for editing in the view.

var usesSingleLineMode: Bool

A Boolean value indicating whether the cell restricts layout and rendering of text to a single line.

