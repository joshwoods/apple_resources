

- AppKit
- NSCell
-  select(withFrame:in:editor:delegate:start:length:) 

Instance Method

# select(withFrame:in:editor:delegate:start:length:)

Selects the specified text range in the cell’s field editor.

macOS

``` source
@MainActor
func select(
    withFrame rect: NSRect,
    in controlView: NSView,
    editor textObj: NSText,
    delegate: Any?,
    start selStart: Int,
    length selLength: Int
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

`selStart`  

The start of the text selection.

`selLength`  

The length of the text range.

## Discussion

This method is similar to edit(withFrame:in:editor:delegate:event:), except that it can be invoked in any situation, not only on a mouse-down event. This method returns without doing anything if `controlView`, `textObj`, or the receiver is `nil`, or if the receiver has no font set for it.

## See Also

### Editing and Selecting Text

func edit(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, event: NSEvent?)

Begins editing of the receiver’s text using the specified field editor.

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

