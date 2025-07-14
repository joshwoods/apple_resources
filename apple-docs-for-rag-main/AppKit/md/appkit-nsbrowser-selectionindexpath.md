

- AppKit
- NSBrowser
-  selectionIndexPath 

Instance Property

# selectionIndexPath

The index path of the item selected in the browser.

macOS 10.6+

``` source
@MainActor
var selectionIndexPath: IndexPath? { get set }
```

## Discussion

When the value of this property is `nil`, there is no selection.

## See Also

### Managing Selection

func selectedCell(inColumn: Int) -> Any?

Returns the last (lowest) cell selected in the given column.

var selectedCells: [NSCell]?

All cells selected in the rightmost column.

func selectAll(Any?)

Selects all cells in the last column of the browser.

func selectedRow(inColumn: Int) -> Int

Returns the row index of the selected cell in the specified column.

func selectRow(Int, inColumn: Int)

Selects the cell at the specified row and column index.

var selectionIndexPaths: [IndexPath]

An array containing the index paths of all items selected in the browser.

