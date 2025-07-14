

- AppKit
- NSTableViewDelegate
-  tableView(\_:shouldTrackCell:for:row:) 

Instance Method

# tableView(\_:shouldTrackCell:for:row:)

Asks the delegate whether the specified cell should be tracked.

macOS 10.5+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    shouldTrackCell cell: NSCell,
    for tableColumn: NSTableColumn?,
    row: Int
) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

`cell`  

The cell to track.

`tableColumn`  

The table column.

`row`  

A row in `tableView`.

## Return Value

true if the cell should be tracked, false otherwise.

## Discussion

In general, only selectable or selected cells can be tracked. If you implement this method, cells that aren’t selectable or selected can be tracked; similarly, cells that are selectable or selected can be set as untracked.

For example, this allows you to have an NSButtonCell object in a table that doesn’t change the selection, but can still be clicked on and tracked.

Note

This method is only valid for NSCell-based table views.

## See Also

### Responding to mouse events

func tableView(NSTableView, didClick: NSTableColumn)

Tells the delegate that the mouse button was clicked in the specified table column, but the column was not dragged.

func tableView(NSTableView, mouseDownInHeaderOf: NSTableColumn)

Tells the delegate that the mouse button was clicked in the specified table column’s header.

