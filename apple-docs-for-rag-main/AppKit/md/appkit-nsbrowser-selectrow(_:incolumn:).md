

- AppKit
- NSBrowser
-  selectRow(\_:inColumn:) 

Instance Method

# selectRow(\_:inColumn:)

Selects the cell at the specified row and column index.

macOS

``` source
@MainActor
func selectRow(
    _ row: Int,
    inColumn column: Int
)
```

## Parameters 

`row`  

The row index of the cell to select.

`column`  

The column index of the cell to select.

## See Also

### Related Documentation

func loadedCell(atRow: Int, column: Int) -> Any?

Loads, if necessary, and returns the cell at the specified row and column location.

### Managing Selection

func selectedCell(inColumn: Int) -> Any?

Returns the last (lowest) cell selected in the given column.

var selectedCells: [NSCell]?

All cells selected in the rightmost column.

func selectAll(Any?)

Selects all cells in the last column of the browser.

func selectedRow(inColumn: Int) -> Int

Returns the row index of the selected cell in the specified column.

var selectionIndexPath: IndexPath?

The index path of the item selected in the browser.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of all items selected in the browser.

