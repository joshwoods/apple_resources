

- AppKit
- NSGridView
-  addColumn(with:) 

Instance Method

# addColumn(with:)

Adds a new column containing the array of views.

macOS 10.12+

``` source
@MainActor
func addColumn(with views: [NSView]) -> NSGridColumn
```

## Return Value

The newly created grid column.

## See Also

### Adding, Removing, and Moving Columns

func insertColumn(at: Int, with: [NSView]) -> NSGridColumn

Inserts the array of view objects at the specified index.

func removeColumn(at: Int)

Removes the column from the grid view at the specified index.

func moveColumn(at: Int, to: Int)

Moves the specified column to a new column location.

