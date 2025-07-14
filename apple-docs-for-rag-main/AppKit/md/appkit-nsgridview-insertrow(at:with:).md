

- AppKit
- NSGridView
-  insertRow(at:with:) 

Instance Method

# insertRow(at:with:)

Inserts the array of view objects into the grid view at the index.

macOS 10.12+

``` source
@MainActor
func insertRow(
    at index: Int,
    with views: [NSView]
) -> NSGridRow
```

## See Also

### Adding, Removing, and Moving Rows

func addRow(with: [NSView]) -> NSGridRow

Adds an array of views to a new row.

func removeRow(at: Int)

Removes the row from the grid view at the index.

func moveRow(at: Int, to: Int)

Moves the specified row to the new row location.

