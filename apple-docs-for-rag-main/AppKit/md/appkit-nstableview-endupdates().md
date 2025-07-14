

- AppKit
- NSTableView
-  endUpdates() 

Instance Method

# endUpdates()

Ends the group of updates for the table view.

macOS 10.7+

``` source
@MainActor
func endUpdates()
```

## Discussion

Ends the group of updates for the table view. This method, like beginUpdates(), is nestable. See beginUpdates() for details.

## See Also

### Updating the Table View Arrangement

func beginUpdates()

Begins a group of updates for the table view.

func moveRow(at: Int, to: Int)

Moves the specified row to the new row location using animation.

func insertRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Inserts the rows using the specified animation.

func removeRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Removes the rows using the specified animation.

func row(for: NSView) -> Int

Returns the index of the row for the specified view.

func column(for: NSView) -> Int

Returns the column index for the specified view.

