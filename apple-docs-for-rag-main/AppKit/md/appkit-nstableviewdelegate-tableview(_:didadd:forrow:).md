

- AppKit
- NSTableViewDelegate
-  tableView(\_:didAdd:forRow:) 

Instance Method

# tableView(\_:didAdd:forRow:)

Tells the delegate that a row view was added at the specified row.

macOS 10.7+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    didAdd rowView: NSTableRowView,
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

At this point, the delegate can add extra views, or modify the properties of `rowView`.

Note

This method is only valid for NSView-based table views.

## See Also

### Notification of row views being added or removed

func tableView(NSTableView, didRemove: NSTableRowView, forRow: Int)

Tells the delegate that a row view was removed from the table at the specified row.

