

- AppKit
- NSControl
-  abortEditing() 

Instance Method

# abortEditing()

Terminates the current editing operation and discards any edited text.

macOS

``` source
@MainActor
func abortEditing() -> Bool
```

## Return Value

true if there was a field editor associated with the control; otherwise, false.

## Discussion

If there was a field editor, this method removes the field editor’s delegate.

Because the control discards any edits, it doesn’t call controlTextDidEndEditing(_:).

## See Also

### Managing the Field Editor

func currentEditor() -> NSText?

Returns the current field editor for the control.

func validateEditing()

Validates changes to any user-typed text.

func edit(withFrame: NSRect, editor: NSText, delegate: Any?, event: NSEvent)

Begins editing of the receiver’s text using the specified field editor.

func endEditing(NSText)

Ends the editing of text in the receiver using the specified field editor.

func select(withFrame: NSRect, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the receiver’s field editor.

