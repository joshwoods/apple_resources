

- AppKit
- NSControl
-  validateEditing() 

Instance Method

# validateEditing()

Validates changes to any user-typed text.

macOS

``` source
@MainActor
func validateEditing()
```

## Discussion

Validation sets the object value of the cell to the current contents of the cell’s editor (the NSText object used for editing), storing it as a simple NSString or an attributed string object based on the attributes of the editor.

## See Also

### Managing the Field Editor

func abortEditing() -> Bool

Terminates the current editing operation and discards any edited text.

func currentEditor() -> NSText?

Returns the current field editor for the control.

func edit(withFrame: NSRect, editor: NSText, delegate: Any?, event: NSEvent)

Begins editing of the receiver’s text using the specified field editor.

func endEditing(NSText)

Ends the editing of text in the receiver using the specified field editor.

func select(withFrame: NSRect, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the receiver’s field editor.

