

- AppKit
- NSControl
-  select(withFrame:editor:delegate:start:length:) 

Instance Method

# select(withFrame:editor:delegate:start:length:)

Selects the specified text range in the receiver’s field editor.

macOS 10.10+

``` source
@MainActor
func select(
    withFrame rect: NSRect,
    editor textObj: NSText,
    delegate: Any?,
    start selStart: Int,
    length selLength: Int
)
```

## Parameters 

`rect`  

The bounding rectangle of the control’s cell.

`textObj`  

The field editor to use.

`delegate`  

The object to use as a delegate for the field editor. This delegate object receives various NSText delegation and notification methods during the course of editing the cell’s contents.

`selStart`  

The start of the text selection.

`selLength`  

The length of the text range.

## Discussion

This method is similar to edit(withFrame:editor:delegate:event:), except that it can be invoked in any situation, not only on a mouse-down event. This method returns without doing anything if `textObj` or the receiver is `nil`, or if the receiver has no font set for it.

## See Also

### Managing the Field Editor

func abortEditing() -> Bool

Terminates the current editing operation and discards any edited text.

func currentEditor() -> NSText?

Returns the current field editor for the control.

func validateEditing()

Validates changes to any user-typed text.

func edit(withFrame: NSRect, editor: NSText, delegate: Any?, event: NSEvent)

Begins editing of the receiver’s text using the specified field editor.

func endEditing(NSText)

Ends the editing of text in the receiver using the specified field editor.

