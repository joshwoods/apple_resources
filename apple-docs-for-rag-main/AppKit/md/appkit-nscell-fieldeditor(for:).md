

- AppKit
- NSCell
-  fieldEditor(for:) 

Instance Method

# fieldEditor(for:)

Returns a custom field editor for editing in the view.

macOS 10.6+

``` source
@MainActor
func fieldEditor(for controlView: NSView) -> NSTextView?
```

## Parameters 

`controlView`  

The view containing cells that require a custom field editor.

## Return Value

A custom field editor. The field editor must have isFieldEditor set to true.

## Discussion

This is an override point for `NSCell` subclasses designed to use their own custom field editors. This message is sent to the selected cell of `aControlView` using the NSWindow method in fieldEditor(_:for:).

Returning non-`nil` from this method indicates skipping the standard field editor querying processes including windowWillReturnFieldEditor(_:to:) delegation.

The default implementation returns `nil`.

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

var wantsNotificationForMarkedText: Bool

A Boolean value indicating whether the cell’s field editor should post text change notifications.

var usesSingleLineMode: Bool

A Boolean value indicating whether the cell restricts layout and rendering of text to a single line.

