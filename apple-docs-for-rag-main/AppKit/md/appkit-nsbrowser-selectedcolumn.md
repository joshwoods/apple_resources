

- AppKit
- NSBrowser
-  selectedColumn 

Instance Property

# selectedColumn

The index of the last column with a selected item.

macOS

``` source
@MainActor
var selectedColumn: Int { get }
```

## Discussion

When the value of this property is `-1`, there is no column selected.

## See Also

### Related Documentation

func selectAll(Any?)

Selects all cells in the last column of the browser.

func column(of: NSMatrix) -> Int

Returns the column number in which the given matrix is located.

Deprecated

### Managing Columns

func addColumn()

Adds a column to the right of the last column.

var lastColumn: Int

The index of the last column loaded.

var firstVisibleColumn: Int

The index of the first visible column.

var numberOfVisibleColumns: Int

The number of visible columns.

var lastVisibleColumn: Int

The index of the last visible column.

func validateVisibleColumns()

Validates the browser’s visible columns.

var isLoaded: Bool

A Boolean that indicates whether column 0 is loaded.

func loadColumnZero()

Loads column 0; unloads previously loaded columns.

func reloadColumn(Int)

Reloads the given column.

