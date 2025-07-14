

- AppKit
- NSBrowser
-  isLeafItem(\_:) 

Instance Method

# isLeafItem(\_:)

Returns whether the specified item is a leaf item.

macOS 10.6+

``` source
@MainActor
func isLeafItem(_ item: Any?) -> Bool
```

## Parameters 

`item`  

The item to be checked.

## Return Value

true if the item is a leaf item; otherwise, false.

## Discussion

This method may return false if the item has never been displayed in the browser or accessed via item(at:). Overriding this method has no effect. It may be used only if the browser’s delegate implements the item data source methods.

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

func parentForItems(inColumn: Int) -> Any?

Returns the item that contains the children located in the specified column.

