

- AppKit
- NSBrowser
-  item(atRow:inColumn:) 

Instance Method

# item(atRow:inColumn:)

Returns the item located at the specified row and column.

macOS 10.6+

``` source
@MainActor
func item(
    atRow row: Int,
    inColumn column: Int
) -> Any?
```

## Parameters 

`row`  

The row of the item.

`column`  

The column of the item.

## Return Value

The item.

## See Also

### Accessing Components

func loadedCell(atRow: Int, column: Int) -> Any?

Loads, if necessary, and returns the cell at the specified row and column location.

func editItem(at: IndexPath, with: NSEvent?, select: Bool)

Begins editing the item at the specified path.

func item(at: IndexPath) -> Any?

Returns the item at the specified index path.

func indexPath(forColumn: Int) -> IndexPath

Returns the index path of the item whose children are displayed in the given column.

func isLeafItem(Any?) -> Bool

Returns whether the specified item is a leaf item.

func parentForItems(inColumn: Int) -> Any?

Returns the item that contains the children located in the specified column.

