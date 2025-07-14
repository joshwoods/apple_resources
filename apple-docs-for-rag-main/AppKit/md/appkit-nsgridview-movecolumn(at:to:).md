

- AppKit
- NSGridView
-  moveColumn(at:to:) 

Instance Method

# moveColumn(at:to:)

Moves the specified column to a new column location.

macOS 10.12+

``` source
@MainActor
func moveColumn(
    at fromIndex: Int,
    to toIndex: Int
)
```

## See Also

### Adding, Removing, and Moving Columns

func addColumn(with: [NSView]) -> NSGridColumn

Adds a new column containing the array of views.

func insertColumn(at: Int, with: [NSView]) -> NSGridColumn

Inserts the array of view objects at the specified index.

func removeColumn(at: Int)

Removes the column from the grid view at the specified index.

