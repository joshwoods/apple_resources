

- AppKit
- NSGridView
-  addRow(with:) 

Instance Method

# addRow(with:)

Adds an array of views to a new row.

macOS 10.12+

``` source
@MainActor
func addRow(with views: [NSView]) -> NSGridRow
```

## Discussion

You can insert and remove rows and columns dynamically in a grid view. The grid is enlarged as needed to hold the specified views.

## See Also

### Adding, Removing, and Moving Rows

func insertRow(at: Int, with: [NSView]) -> NSGridRow

Inserts the array of view objects into the grid view at the index.

func removeRow(at: Int)

Removes the row from the grid view at the index.

func moveRow(at: Int, to: Int)

Moves the specified row to the new row location.

