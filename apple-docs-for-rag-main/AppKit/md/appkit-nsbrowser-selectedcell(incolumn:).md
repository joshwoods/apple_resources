

- AppKit
- NSBrowser
-  selectedCell(inColumn:) 

Instance Method

# selectedCell(inColumn:)

Returns the last (lowest) cell selected in the given column.

macOS

``` source
@MainActor
func selectedCell(inColumn column: Int) -> Any?
```

## Parameters 

`column`  

The column whose last selected cell is to be returned.

## Return Value

The last (or lowest) selected cell. Returns `nil` if there is no selection.

## See Also

### Related Documentation

func loadedCell(atRow: Int, column: Int) -> Any?

Loads, if necessary, and returns the cell at the specified row and column location.

### Managing Selection

var selectedCells: [NSCell]?

All cells selected in the rightmost column.

func selectAll(Any?)

Selects all cells in the last column of the browser.

func selectedRow(inColumn: Int) -> Int

Returns the row index of the selected cell in the specified column.

func selectRow(Int, inColumn: Int)

Selects the cell at the specified row and column index.

var selectionIndexPath: IndexPath?

The index path of the item selected in the browser.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of all items selected in the browser.

