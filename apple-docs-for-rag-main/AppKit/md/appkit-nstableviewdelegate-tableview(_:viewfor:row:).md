

- AppKit
- NSTableViewDelegate
-  tableView(\_:viewFor:row:) 

Instance Method

# tableView(\_:viewFor:row:)

Asks the delegate for a view to display the specified row and column.

macOS 10.7+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    viewFor tableColumn: NSTableColumn?,
    row: Int
) -> NSView?
```

## Parameters 

`tableView`  

The table view that sent the message.

`tableColumn`  

The table column. (If the row is a group row, `tableColumn` is `nil`.)

`row`  

The row index.

## Return Value

The view to display the specified column and row. If you return `nil`, a view will not be shown at that location.

## Discussion

This method is required if you want to use NSView objects instead of NSCell objects for the cells within a table view. Cells and views can’t be mixed within the same table view.

It’s recommended that the implementation of this method first call the NSTableView method makeView(withIdentifier:owner:) passing, respectively, the `tableColumn` parameter’s identifier and `self` as the owner to attempt to reuse a view that is no longer visible or automatically unarchive an associated prototype view for that identifier. The `frame` of the view returned by this method is not important, and it will be automatically set by the table.

The view’s properties should be properly set up before returning the result.

When using Cocoa bindings, this method is optional if at least one identifier has been associated with the table view at design time. (Note that a view’s identifier must be the same as the identifier of its column. An easy way to achieve this is to use the Automatic identifier setting in Interface Builder.) If this method isn’t implemented, the table will automatically call the NSTableView method makeView(withIdentifier:owner:) with the `tableColumn` parameter’s identifier and the table view’s `delegate` as parameters, to attempt to reuse a previous view, or automatically unarchive a prototype associated with the table view. If this method is implemented, you can set up properties that aren’t using bindings.

The autoresizing mask of the returned view will automatically be set to height to resize properly on row height changes.

## See Also

### Related Documentation

Table View Programming Guide for Mac

Drag and Drop Programming Topics

### Providing views for rows and columns

func tableView(NSTableView, rowViewForRow: Int) -> NSTableRowView?

Asks the delegate for a view to display the specified row.

