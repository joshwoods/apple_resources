

- AppKit
- NSBrowser
-  loadedCell(atRow:column:) 

Instance Method

# loadedCell(atRow:column:)

Loads, if necessary, and returns the cell at the specified row and column location.

macOS

``` source
@MainActor
func loadedCell(
    atRow row: Int,
    column col: Int
) -> Any?
```

## Parameters 

`row`  

The row index of the cell to return.

`col`  

The column index of the cell to return.

## See Also

### Related Documentation

func selectRow(Int, inColumn: Int)

Selects the cell at the specified row and column index.

func selectedCell(inColumn: Int) -> Any?

Returns the last (lowest) cell selected in the given column.

### Accessing Components

func editItem(at: IndexPath, with: NSEvent?, select: Bool)

Begins editing the item at the specified path.

func item(at: IndexPath) -> Any?

Returns the item at the specified index path.

func item(atRow: Int, inColumn: Int) -> Any?

Returns the item located at the specified row and column.

func indexPath(forColumn: Int) -> IndexPath

Returns the index path of the item whose children are displayed in the given column.

func isLeafItem(Any?) -> Bool

Returns whether the specified item is a leaf item.

func parentForItems(inColumn: Int) -> Any?

Returns the item that contains the children located in the specified column.

