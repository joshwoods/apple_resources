

- AppKit
- NSGridView
-  insertColumn(at:with:) 

Instance Method

# insertColumn(at:with:)

Inserts the array of view objects at the specified index.

macOS 10.12+

``` source
@MainActor
func insertColumn(
    at index: Int,
    with views: [NSView]
) -> NSGridColumn
```

## See Also

### Adding, Removing, and Moving Columns

func addColumn(with: [NSView]) -> NSGridColumn

Adds a new column containing the array of views.

func removeColumn(at: Int)

Removes the column from the grid view at the specified index.

func moveColumn(at: Int, to: Int)

Moves the specified column to a new column location.

