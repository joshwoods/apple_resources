

- AppKit
- NSTableViewDelegate
-  tableViewColumnDidMove(\_:) 

Instance Method

# tableViewColumnDidMove(\_:)

Tells the delegate that a table column was moved by user action.

macOS 10.10+

``` source
@MainActor
optional func tableViewColumnDidMove(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named columnDidMoveNotification.

## See Also

### Moving and resizing columns

func tableView(NSTableView, shouldReorderColumn: Int, toColumn: Int) -> Bool

Asks the delegate to allow or prohibit the specified column to be dragged to a new location.

func tableView(NSTableView, didDrag: NSTableColumn)

Tells the delegate that the specified table column was dragged.

func tableViewColumnDidResize(Notification)

Tells the delegate that a table column was resized.

