

- AppKit
- NSMatrix
-  setState(\_:atRow:column:) 

Instance Method

# setState(\_:atRow:column:)

Sets the state of the cell at specified location.

macOS

``` source
@MainActor
func setState(
    _ value: Int,
    atRow row: Int,
    column col: Int
)
```

## Parameters 

`value`  

The value to assign to the cell.

`row`  

The row in which the cell is located.

`col`  

The column in which the cell is located.

## Discussion

For radio-mode matrices, if `value` is nonzero the specified cell is selected before its state is set to `value`. If `value` is 0 and the receiver is a radio-mode matrix, the currently selected cell is deselected (providing that empty selection is allowed).

This method redraws the affected cell.

## See Also

### Related Documentation

var state: NSControl.StateValue

The cell’s current state.

func selectCell(atRow: Int, column: Int)

Selects the cell at the specified row and column within the receiver.

var allowsEmptySelection: Bool

A Boolean that indicates whether a radio-mode matrix supports an empty selection.

### Managing Attributes of Individual Cells

func setToolTip(String?, for: NSCell)

Sets the tooltip for the cell.

func toolTip(for: NSCell) -> String?

Returns the tooltip for the specified cell.

