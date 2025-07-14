

- AppKit
- NSBrowser
-  parentForItems(inColumn:) 

Instance Method

# parentForItems(inColumn:)

Returns the item that contains the children located in the specified column.

macOS 10.6+

``` source
@MainActor
func parentForItems(inColumn column: Int) -> Any?
```

## Parameters 

`column`  

The column.

## Return Value

The parent item for the specified column.

## See Also

### Accessing Components

func loadedCell(atRow: Int, column: Int) -> Any?

Loads, if necessary, and returns the cell at the specified row and column location.

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

