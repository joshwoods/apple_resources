

- AppKit
- NSTableView
-  removeRows(at:withAnimation:) 

Instance Method

# removeRows(at:withAnimation:)

Removes the rows using the specified animation.

macOS 10.7+

``` source
@MainActor
func removeRows(
    at indexes: IndexSet,
    withAnimation animationOptions: NSTableView.AnimationOptions = []
)
```

## Parameters 

`indexes`  

An index set containing the rows to remove.

`animationOptions`  

The animation displayed during the insert. See NSTableView.AnimationOptions for the possible values that can be combined using the C bitwise OR operator.

## Discussion

This method deletes from the table the rows represented at `indexes` and automatically decreases numberOfRows by the count of `indexes`.

The row indexes should be with respect to the current state displayed in the table view, and not the final state, because the specified rows do not exist in the final state.

Calling this method multiple times within the same beginUpdates() and endUpdates() block is allowed, and changes are processed incrementally.

Changes are processed incrementally as the insertRows(at:withAnimation:), removeRows(at:withAnimation:), and the moveRow(at:to:) methods are called. It is acceptable to delete row `0` multiple times, as long as there is still a row available.

Note

NSCell-based table views must first call beginUpdates() before calling this method.

## See Also

### Updating the Table View Arrangement

func beginUpdates()

Begins a group of updates for the table view.

func endUpdates()

Ends the group of updates for the table view.

func moveRow(at: Int, to: Int)

Moves the specified row to the new row location using animation.

func insertRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Inserts the rows using the specified animation.

func row(for: NSView) -> Int

Returns the index of the row for the specified view.

func column(for: NSView) -> Int

Returns the column index for the specified view.

