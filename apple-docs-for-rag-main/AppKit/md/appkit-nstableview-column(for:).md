

- AppKit
- NSTableView
-  column(for:) 

Instance Method

# column(for:)

Returns the column index for the specified view.

macOS 10.7+

``` source
@MainActor
func column(for view: NSView) -> Int
```

## Parameters 

`view`  

The view for which to retrieve the column.

## Return Value

The index of the column containing `view` in the tableColumns array. This method returns `-1` if the view is not in the table view. This method may also return `-1` if the row containing the view is being animated away, such as during the deletion of a row.

## Discussion

This method is typically called in the action method of an `NSButton` (or `NSControl`) to find out what row (and column) the action should be performed on.

The implementation is `O(n)` where *n* is the number of visible rows, so this method should generally not be called within a loop.

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

func removeRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Removes the rows using the specified animation.

func row(for: NSView) -> Int

Returns the index of the row for the specified view.

