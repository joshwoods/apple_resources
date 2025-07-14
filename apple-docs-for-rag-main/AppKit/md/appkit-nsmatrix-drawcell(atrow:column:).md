

- AppKit
- NSMatrix
-  drawCell(atRow:column:) 

Instance Method

# drawCell(atRow:column:)

Displays the cell at the specified row and column.

macOS

``` source
@MainActor
func drawCell(
    atRow row: Int,
    column col: Int
)
```

## Parameters 

`row`  

The row containing the cell to draw.

`col`  

The column containing the cell to draw.

## See Also

### Related Documentation

func drawCell(NSCell)

Draws the specified cell, as long as it belongs to the receiver.

func drawCellInside(NSCell)

Draws the inside of the receiver’s cell (the area within the bezel or border)

### Displaying and Highlighting Cells

func highlightCell(Bool, atRow: Int, column: Int)

Highlights or unhighlights the cell at the specified row and column location.

