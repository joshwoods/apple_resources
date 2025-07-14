

- AppKit
- NSTableViewDelegate
-  tableView(\_:rowViewForRow:) 

Instance Method

# tableView(\_:rowViewForRow:)

Asks the delegate for a view to display the specified row.

macOS 10.7+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    rowViewForRow row: Int
) -> NSTableRowView?
```

## Parameters 

`tableView`  

The table view that sent the message.

`row`  

The row index.

## Return Value

An instance or subclass of NSTableRowView. If `nil` is returned, an NSTableRowView instance will be created and used.

## Discussion

The delegate can implement this method to return a custom NSTableRowView for `row`.

The reuse queue can be used in the same way as documented in tableView(_:viewFor:row:). The returned view will have attributes properly set to it before it’s added to the `tableView`.

Note

This method is only valid for NSView-based table views.

## See Also

### Providing views for rows and columns

func tableView(NSTableView, viewFor: NSTableColumn?, row: Int) -> NSView?

Asks the delegate for a view to display the specified row and column.

