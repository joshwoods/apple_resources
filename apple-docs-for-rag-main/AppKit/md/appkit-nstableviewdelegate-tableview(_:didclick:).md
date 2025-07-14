

- AppKit
- NSTableViewDelegate
-  tableView(\_:didClick:) 

Instance Method

# tableView(\_:didClick:)

Tells the delegate that the mouse button was clicked in the specified table column, but the column was not dragged.

macOS

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    didClick tableColumn: NSTableColumn
)
```

## Parameters 

`tableView`  

The table view that sent the message.

`tableColumn`  

The table column.

## See Also

### Responding to mouse events

func tableView(NSTableView, mouseDownInHeaderOf: NSTableColumn)

Tells the delegate that the mouse button was clicked in the specified table column’s header.

func tableView(NSTableView, shouldTrackCell: NSCell, for: NSTableColumn?, row: Int) -> Bool

Asks the delegate whether the specified cell should be tracked.

