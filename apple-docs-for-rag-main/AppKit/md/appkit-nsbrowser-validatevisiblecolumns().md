

- AppKit
- NSBrowser
-  validateVisibleColumns() 

Instance Method

# validateVisibleColumns()

Validates the browser’s visible columns.

macOS

``` source
@MainActor
func validateVisibleColumns()
```

## Discussion

This method invokes the delegate method browser(_:isColumnValid:)

## See Also

### Managing Columns

func addColumn()

Adds a column to the right of the last column.

var selectedColumn: Int

The index of the last column with a selected item.

var lastColumn: Int

The index of the last column loaded.

var firstVisibleColumn: Int

The index of the first visible column.

var numberOfVisibleColumns: Int

The number of visible columns.

var lastVisibleColumn: Int

The index of the last visible column.

var isLoaded: Bool

A Boolean that indicates whether column 0 is loaded.

func loadColumnZero()

Loads column 0; unloads previously loaded columns.

func reloadColumn(Int)

Reloads the given column.

