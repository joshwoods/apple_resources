

- AppKit
- NSGridView
-  removeColumn(at:) 

Instance Method

# removeColumn(at:)

Removes the column from the grid view at the specified index.

macOS 10.12+

``` source
@MainActor
func removeColumn(at index: Int)
```

## See Also

### Adding, Removing, and Moving Columns

func addColumn(with: [NSView]) -> NSGridColumn

Adds a new column containing the array of views.

func insertColumn(at: Int, with: [NSView]) -> NSGridColumn

Inserts the array of view objects at the specified index.

func moveColumn(at: Int, to: Int)

Moves the specified column to a new column location.

