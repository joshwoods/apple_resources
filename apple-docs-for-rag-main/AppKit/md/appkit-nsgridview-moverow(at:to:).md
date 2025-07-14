

- AppKit
- NSGridView
-  moveRow(at:to:) 

Instance Method

# moveRow(at:to:)

Moves the specified row to the new row location.

macOS 10.12+

``` source
@MainActor
func moveRow(
    at fromIndex: Int,
    to toIndex: Int
)
```

## See Also

### Adding, Removing, and Moving Rows

func addRow(with: [NSView]) -> NSGridRow

Adds an array of views to a new row.

func insertRow(at: Int, with: [NSView]) -> NSGridRow

Inserts the array of view objects into the grid view at the index.

func removeRow(at: Int)

Removes the row from the grid view at the index.

