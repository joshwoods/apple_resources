

- AppKit
- NSMatrix
-  selectText(atRow:column:) 

Instance Method

# selectText(atRow:column:)

Selects the text in the cell at the specified location and returns the cell.

macOS

``` source
@MainActor
func selectText(
    atRow row: Int,
    column col: Int
) -> NSCell?
```

## Parameters 

`row`  

The row containing the text to select.

`col`  

The column containing the text to select.

## Return Value

If it is both editable and selectable, the cell at the specified row and column. If the cell at the specified location, is either not editable or not selectable, this method does nothing and returns nil. If `row` and `column` indicate a cell that is outside the receiver, this method does nothing and returns the receiver.

## See Also

### Editing Text in Cells

func selectText(Any?)

Selects text in the currently selected cell or in the key cell.

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

