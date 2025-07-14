

- AppKit
- NSMatrix
-  selectText(\_:) 

Instance Method

# selectText(\_:)

Selects text in the currently selected cell or in the key cell.

macOS

``` source
@MainActor
func selectText(_ sender: Any?)
```

## Discussion

If the currently selected cell is editable and enabled, its text is selected. Otherwise, the key cell is selected.

## See Also

### Related Documentation

func selectText(Any?)

Ends editing in the text field and, if it’s selectable, selects the entire text content.

var keyCell: NSCell?

The cell that will be clicked when the user presses the Space bar.

### Editing Text in Cells

func selectText(atRow: Int, column: Int) -> NSCell?

Selects the text in the cell at the specified location and returns the cell.

func textShouldBeginEditing(NSText) -> Bool

Requests permission to begin editing text.

func textDidBeginEditing(Notification)

Invoked when there’s a change in the text after the receiver gains first responder status.

func textDidChange(Notification)

Invoked when a key-down event or paste operation occurs that changes the receiver’s contents.

func textShouldEndEditing(NSText) -> Bool

Requests permission to end editing.

func textDidEndEditing(Notification)

Invoked when text editing ends.

