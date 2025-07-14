

- AppKit
- NSCell
-  wantsNotificationForMarkedText 

Instance Property

# wantsNotificationForMarkedText

A Boolean value indicating whether the cell’s field editor should post text change notifications.

macOS

``` source
@MainActor
var wantsNotificationForMarkedText: Bool { get }
```

## Discussion

When the value of this property is true, the field editor should post text notification changes while editing marked text. When the value is NO, the field editor should delay notifications until the marked text is confirmed.

The default value of this property is false. Subclasses can override the property and change the value as appropriate.

## See Also

### Editing and Selecting Text

func edit(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, event: NSEvent?)

Begins editing of the receiver’s text using the specified field editor.

func select(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the cell’s field editor.

var sendsActionOnEndEditing: Bool

A Boolean value indicating whether the cell’s control object sends its action message when the user finishes editing the cell’s text.

func endEditing(NSText)

Ends the editing of text in the receiver using the specified field editor.

func fieldEditor(for: NSView) -> NSTextView?

Returns a custom field editor for editing in the view.

var usesSingleLineMode: Bool

A Boolean value indicating whether the cell restricts layout and rendering of text to a single line.

