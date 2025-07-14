

- AppKit
- NSTableViewDelegate
-  tableViewColumnDidResize(\_:) 

Instance Method

# tableViewColumnDidResize(\_:)

Tells the delegate that a table column was resized.

macOS 10.10+

``` source
@MainActor
optional func tableViewColumnDidResize(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named columnDidResizeNotification.

## See Also

### Moving and resizing columns

func tableView(NSTableView, shouldReorderColumn: Int, toColumn: Int) -> Bool

Asks the delegate to allow or prohibit the specified column to be dragged to a new location.

func tableView(NSTableView, didDrag: NSTableColumn)

Tells the delegate that the specified table column was dragged.

func tableViewColumnDidMove(Notification)

Tells the delegate that a table column was moved by user action.

