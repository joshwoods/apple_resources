

- AppKit
- NSTableView
-  moveRow(at:to:) 

Instance Method

# moveRow(at:to:)

Moves the specified row to the new row location using animation.

macOS 10.7+

``` source
@MainActor
func moveRow(
    at oldIndex: Int,
    to newIndex: Int
)
```

## Parameters 

`oldIndex`  

Initial row index.

`newIndex`  

New row index.

## Discussion

This is similar to removing a row at `oldIndex` and inserting it at `newIndex`, except the same view is used and simply has its position updated to the new location.

Changes happen incrementally as they are sent to the table, so as soon as this method is called the row can be considered moved. However the underlying view is not moved until endUpdates() has been called.

This method can be called multiple times within the same beginUpdates() and endUpdates() block.

Note

NSCell-based table views must first call beginUpdates() before calling this method.

## See Also

### Updating the Table View Arrangement

func beginUpdates()

Begins a group of updates for the table view.

func endUpdates()

Ends the group of updates for the table view.

func insertRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Inserts the rows using the specified animation.

func removeRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Removes the rows using the specified animation.

func row(for: NSView) -> Int

Returns the index of the row for the specified view.

func column(for: NSView) -> Int

Returns the column index for the specified view.

