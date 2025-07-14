

- AppKit
- NSBrowser
-  selectAll(\_:) 

Instance Method

# selectAll(\_:)

Selects all cells in the last column of the browser.

macOS

``` source
@MainActor
func selectAll(_ sender: Any?)
```

## See Also

### Related Documentation

var selectedColumn: Int

The index of the last column with a selected item.

### Managing Selection

func selectedCell(inColumn: Int) -> Any?

Returns the last (lowest) cell selected in the given column.

var selectedCells: [NSCell]?

All cells selected in the rightmost column.

func selectedRow(inColumn: Int) -> Int

Returns the row index of the selected cell in the specified column.

func selectRow(Int, inColumn: Int)

Selects the cell at the specified row and column index.

var selectionIndexPath: IndexPath?

The index path of the item selected in the browser.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of all items selected in the browser.

