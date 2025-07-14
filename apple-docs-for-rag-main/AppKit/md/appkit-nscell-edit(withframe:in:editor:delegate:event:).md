

- AppKit
- NSCell
-  edit(withFrame:in:editor:delegate:event:) 

Instance Method

# edit(withFrame:in:editor:delegate:event:)

Begins editing of the receiver’s text using the specified field editor.

macOS

``` source
@MainActor
func edit(
    withFrame rect: NSRect,
    in controlView: NSView,
    editor textObj: NSText,
    delegate: Any?,
    event: NSEvent?
)
```

## Parameters 

`rect`  

The bounding rectangle of the cell.

`controlView`  

The control that manages the cell.

`textObj`  

The field editor to use for editing the cell.

`delegate`  

The object to use as a delegate for the field editor (`textObj` parameter). This delegate object receives various `NSText` delegation and notification methods during the course of editing the cell’s contents.

`event`  

The `NSLeftMouseDown` event that initiated the editing behavior.

## Discussion

If the receiver isn’t a text-type `NSCell` object, no editing is performed. Otherwise, the field editor (`textObj`) is sized to `aRect` and its superview is set to `controlView`, so it exactly covers the receiver. The field editor is then activated and editing begins. It’s the responsibility of the delegate to end editing when responding to textShouldEndEditing(_:). Upon ending the editing session, the delegate should remove any data from the field editor.

## See Also

### Editing and Selecting Text

func select(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the cell’s field editor.

var sendsActionOnEndEditing: Bool

A Boolean value indicating whether the cell’s control object sends its action message when the user finishes editing the cell’s text.

func endEditing(NSText)

Ends the editing of text in the receiver using the specified field editor.

var wantsNotificationForMarkedText: Bool

A Boolean value indicating whether the cell’s field editor should post text change notifications.

func fieldEditor(for: NSView) -> NSTextView?

Returns a custom field editor for editing in the view.

var usesSingleLineMode: Bool

A Boolean value indicating whether the cell restricts layout and rendering of text to a single line.

