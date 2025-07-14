

- AppKit
- NSMatrix
-  setToolTip(\_:for:) 

Instance Method

# setToolTip(\_:for:)

Sets the tooltip for the cell.

macOS

``` source
@MainActor
func setToolTip(
    _ toolTipString: String?,
    for cell: NSCell
)
```

## Parameters 

`toolTipString`  

The string to use as the cell’s tooltip (or help tag).

`cell`  

The cell to which to assign the tooltip.

## See Also

### Managing Attributes of Individual Cells

func setState(Int, atRow: Int, column: Int)

Sets the state of the cell at specified location.

func toolTip(for: NSCell) -> String?

Returns the tooltip for the specified cell.

