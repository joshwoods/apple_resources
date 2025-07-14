

- AppKit
- NSTableViewDelegate
-  tableView(\_:didDrag:) 

Instance Method

# tableView(\_:didDrag:)

Tells the delegate that the specified table column was dragged.

macOS

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    didDrag tableColumn: NSTableColumn
)
```

## Parameters 

`tableView`  

The table view that sent the message.

`tableColumn`  

The table column.

## Discussion

Specifically, this method is sent when the mouse button goes up in `tableView` and `tableColumn` has been dragged during the time the mouse button was down. In macOS 10.5 and later the dragged column is sent to the delegate. (In earlier versions of macOS the table column that’s currently located at the dragged column’s original index is sent.)

## See Also

### Moving and resizing columns

func tableView(NSTableView, shouldReorderColumn: Int, toColumn: Int) -> Bool

Asks the delegate to allow or prohibit the specified column to be dragged to a new location.

func tableViewColumnDidMove(Notification)

Tells the delegate that a table column was moved by user action.

func tableViewColumnDidResize(Notification)

Tells the delegate that a table column was resized.

