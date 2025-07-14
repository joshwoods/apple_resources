

- AppKit
- NSBrowser
-  indexPath(forColumn:) 

Instance Method

# indexPath(forColumn:)

Returns the index path of the item whose children are displayed in the given column.

macOS 10.6+

``` source
@MainActor
func indexPath(forColumn column: Int) -> IndexPath
```

## Parameters 

`column`  

The column to find the index path for.

## Return Value

The index path of the column.

## Discussion

This method can only be used if the delegate implements the item data source methods.

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

func isLeafItem(Any?) -> Bool

Returns whether the specified item is a leaf item.

func parentForItems(inColumn: Int) -> Any?

Returns the item that contains the children located in the specified column.

