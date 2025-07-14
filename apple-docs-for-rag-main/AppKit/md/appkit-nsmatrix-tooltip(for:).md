

- AppKit
- NSMatrix
-  toolTip(for:) 

Instance Method

# toolTip(for:)

Returns the tooltip for the specified cell.

macOS

``` source
@MainActor
func toolTip(for cell: NSCell) -> String?
```

## Parameters 

`cell`  

The cell for which to return the tooltip.

## Return Value

The string used as the cell’s tooltip.

## See Also

### Managing Attributes of Individual Cells

func setState(Int, atRow: Int, column: Int)

Sets the state of the cell at specified location.

func setToolTip(String?, for: NSCell)

Sets the tooltip for the cell.

