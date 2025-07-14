

- AppKit
- NSBrowser
-  selectedRow(inColumn:) 

Instance Method

# selectedRow(inColumn:)

Returns the row index of the selected cell in the specified column.

macOS

``` source
@MainActor
func selectedRow(inColumn column: Int) -> Int
```

## Parameters 

`column`  

The column index specifying the column for which to return the selected row.

## Return Value

The row index of the selected cell in the specified column. Returns `-1` if there is no selection.

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

func selectRow(Int, inColumn: Int)

Selects the cell at the specified row and column index.

var selectionIndexPath: IndexPath?

The index path of the item selected in the browser.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of all items selected in the browser.

