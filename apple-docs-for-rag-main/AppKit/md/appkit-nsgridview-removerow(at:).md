

- AppKit
- NSGridView
-  removeRow(at:) 

Instance Method

# removeRow(at:)

Removes the row from the grid view at the index.

macOS 10.12+

``` source
@MainActor
func removeRow(at index: Int)
```

## See Also

### Adding, Removing, and Moving Rows

func addRow(with: [NSView]) -> NSGridRow

Adds an array of views to a new row.

func insertRow(at: Int, with: [NSView]) -> NSGridRow

Inserts the array of view objects into the grid view at the index.

func moveRow(at: Int, to: Int)

Moves the specified row to the new row location.

