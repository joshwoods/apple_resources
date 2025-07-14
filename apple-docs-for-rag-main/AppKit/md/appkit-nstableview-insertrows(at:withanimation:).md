

- AppKit
- NSTableView
-  insertRows(at:withAnimation:) 

Instance Method

# insertRows(at:withAnimation:)

Inserts the rows using the specified animation.

macOS 10.7+

``` source
@MainActor
func insertRows(
    at indexes: IndexSet,
    withAnimation animationOptions: NSTableView.AnimationOptions = []
)
```

## Parameters 

`indexes`  

The final positions of the new rows to be inserted.

`animationOptions`  

The animation displayed during the insert. See NSTableView.AnimationOptions for the possible values that can be combined using the C bitwise OR operator.

## Discussion

The numberOfRows in the table view is automatically increased by the count of `indexes`.

Calling this method multiple times within the same beginUpdates() and endUpdates() block is allowed, and changes are processed incrementally.

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

func removeRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Removes the rows using the specified animation.

func row(for: NSView) -> Int

Returns the index of the row for the specified view.

func column(for: NSView) -> Int

Returns the column index for the specified view.

