

- AppKit
- NSMatrix
-  highlightCell(\_:atRow:column:) 

Instance Method

# highlightCell(\_:atRow:column:)

Highlights or unhighlights the cell at the specified row and column location.

macOS

``` source
@MainActor
func highlightCell(
    _ flag: Bool,
    atRow row: Int,
    column col: Int
)
```

## Parameters 

`flag`  

true to highlight the cell; false to unhighlight the cell.

`row`  

The row containing the cell.

`col`  

The column containing the cell.

## See Also

### Displaying and Highlighting Cells

func drawCell(atRow: Int, column: Int)

Displays the cell at the specified row and column.

