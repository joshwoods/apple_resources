

- AppKit
- NSBrowser
-  item(at:) 

Instance Method

# item(at:)

Returns the item at the specified index path.

macOS 10.6+

``` source
@MainActor
func item(at indexPath: IndexPath) -> Any?
```

## Parameters 

`indexPath`  

The index path of the item to return.

## Return Value

The item.

## Discussion

This method can only be used if the delegate implements the item data source methods. The specified index path must be displayable in the browser.

## See Also

### Accessing Components

func loadedCell(atRow: Int, column: Int) -> Any?

Loads, if necessary, and returns the cell at the specified row and column location.

func editItem(at: IndexPath, with: NSEvent?, select: Bool)

Begins editing the item at the specified path.

func item(atRow: Int, inColumn: Int) -> Any?

Returns the item located at the specified row and column.

func indexPath(forColumn: Int) -> IndexPath

Returns the index path of the item whose children are displayed in the given column.

func isLeafItem(Any?) -> Bool

Returns whether the specified item is a leaf item.

func parentForItems(inColumn: Int) -> Any?

Returns the item that contains the children located in the specified column.

