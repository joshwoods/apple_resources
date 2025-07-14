

- AppKit
- NSControl
-  edit(withFrame:editor:delegate:event:) 

Instance Method

# edit(withFrame:editor:delegate:event:)

Begins editing of the receiver’s text using the specified field editor.

macOS 10.10+

``` source
@MainActor
func edit(
    withFrame rect: NSRect,
    editor textObj: NSText,
    delegate: Any?,
    event: NSEvent
)
```

## Parameters 

`rect`  

The bounding rectangle of the control’s cell.

`textObj`  

The field editor to use.

`delegate`  

The object to use as a delegate for the field editor. This delegate object receives various NSText delegation and notification methods during the course of editing the cell’s contents.

`event`  

The NSLeftMouseDown event that initiated the editing behavior.

## Discussion

For a receiver that is a control with editable text (such as an NSTextField object), the field editor is sized to `aRect` and is then activated and editing begins. It’s the responsibility of the delegate to end editing when responding to control(_:textShouldEndEditing:). Upon ending the editing session, the delegate should remove any data from the field editor.

## See Also

### Managing the Field Editor

func abortEditing() -> Bool

Terminates the current editing operation and discards any edited text.

func currentEditor() -> NSText?

Returns the current field editor for the control.

func validateEditing()

Validates changes to any user-typed text.

func endEditing(NSText)

Ends the editing of text in the receiver using the specified field editor.

func select(withFrame: NSRect, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the receiver’s field editor.

