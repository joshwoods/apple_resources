

- AppKit
- NSControl
-  endEditing(\_:) 

Instance Method

# endEditing(\_:)

Ends the editing of text in the receiver using the specified field editor.

macOS 10.10+

``` source
@MainActor
func endEditing(_ textObj: NSText)
```

## Parameters 

`textObj`  

The field editor currently handling the editing of the cell’s content.

## Discussion

Ends any editing of text that began with a call to edit(withFrame:editor:delegate:event:) or select(withFrame:editor:delegate:start:length:).

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

func select(withFrame: NSRect, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the receiver’s field editor.

