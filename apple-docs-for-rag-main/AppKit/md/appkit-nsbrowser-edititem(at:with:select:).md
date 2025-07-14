

- AppKit
- NSBrowser
-  editItem(at:with:select:) 

Instance Method

# editItem(at:with:select:)

Begins editing the item at the specified path.

macOS 10.6+

``` source
@MainActor
func editItem(
    at indexPath: IndexPath,
    with event: NSEvent?,
    select: Bool
)
```

## Parameters 

`indexPath`  

The path of the item.

`event`  

The event to use when beginning the edit.

`select`  

If true, the cells contents will be selected; if false, they will not be selected.

## See Also

### Accessing Components

func loadedCell(atRow: Int, column: Int) -> Any?

Loads, if necessary, and returns the cell at the specified row and column location.

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

