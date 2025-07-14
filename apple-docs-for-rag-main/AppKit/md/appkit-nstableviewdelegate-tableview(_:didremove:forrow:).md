

- AppKit
- NSTableViewDelegate
-  tableView(\_:didRemove:forRow:) 

Instance Method

# tableView(\_:didRemove:forRow:)

Tells the delegate that a row view was removed from the table at the specified row.

macOS 10.7+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    didRemove rowView: NSTableRowView,
    forRow row: Int
)
```

## Parameters 

`tableView`  

The table view that sent the message.

`rowView`  

The row view.

`row`  

The index of the row.

## Discussion

If `row` equals `-1`, the row is being deleted from the table and is no longer a valid row; otherwise `row` is a valid row that is being removed by being moved off screen.

Note

This method is only valid for NSView-based table views.

## See Also

### Notification of row views being added or removed

func tableView(NSTableView, didAdd: NSTableRowView, forRow: Int)

Tells the delegate that a row view was added at the specified row.

