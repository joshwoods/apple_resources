

- AppKit
- NSTableView
-  beginUpdates() 

Instance Method

# beginUpdates()

Begins a group of updates for the table view.

macOS 10.7+

``` source
@MainActor
func beginUpdates()
```

## Discussion

For NSView-based table views, multiple row changes—that is, insertions, deletions, and moves—are animated simultaneously by surrounding calls to those method calls with beginUpdates() and endUpdates(). These methods are nestable.

The selected rows are maintained during the series of insertions, deletions, moves, and scrolling. If a selected row is deleted, a selection changed notification occurs after removeRows(at:withAnimation:) is called.

It is not necessary to call beginUpdates() and endUpdates() if only one insertion, deletion, or move is occurring and the table view is an NSView-based table view. When using an NSCell-based table view, you must surround any insertion, deletion, or move in an update block for animations to occur.

The main reason for doing a batch update of changes to a table view is to avoid having the table animate unnecessarily.

Note that these methods should be called to reflect changes in your model; they do not make any underlying model changes.

Note

For NSCell-based table views, it is required to call beginUpdates() if you want to animate the insertRows(at:withAnimation:), removeRows(at:withAnimation:), and moveRow(at:to:).

## See Also

### Related Documentation

func removeTableColumn(NSTableColumn)

Removes the specified column from the table view.

### Updating the Table View Arrangement

func endUpdates()

Ends the group of updates for the table view.

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

