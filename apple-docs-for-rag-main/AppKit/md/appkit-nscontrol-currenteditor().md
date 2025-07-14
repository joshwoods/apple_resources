

- AppKit
- NSControl
-  currentEditor() 

Instance Method

# currentEditor()

Returns the current field editor for the control.

macOS

``` source
@MainActor
func currentEditor() -> NSText?
```

## Return Value

The field editor for the current control, or `nil` if the receiver does not have a field editor.

## Discussion

When the receiver is a control displaying editable text (for example, a text field) and it is the first responder, it has a field editor, which is returned by this method. The field editor is a single NSTextView object that is shared among all the controls in a window for light text-editing needs. It is automatically instantiated when needed.

## See Also

### Managing the Field Editor

func abortEditing() -> Bool

Terminates the current editing operation and discards any edited text.

func validateEditing()

Validates changes to any user-typed text.

func edit(withFrame: NSRect, editor: NSText, delegate: Any?, event: NSEvent)

Begins editing of the receiver’s text using the specified field editor.

func endEditing(NSText)

Ends the editing of text in the receiver using the specified field editor.

func select(withFrame: NSRect, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the receiver’s field editor.

