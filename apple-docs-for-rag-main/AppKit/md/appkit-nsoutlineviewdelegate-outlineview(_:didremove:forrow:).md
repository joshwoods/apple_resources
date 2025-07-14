

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:didRemove:forRow:) 

Instance Method

# outlineView(\_:didRemove:forRow:)

Implemented to know when a row view is removed from the table

macOS 10.7+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    didRemove rowView: NSTableRowView,
    forRow row: Int
)
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`rowView`  

The row view that was removed.

`row`  

The number of the row that was removed due to being moved offscreen, or `-1` if the row was removed from the table so it is no longer valid.

## Discussion

The removed `rowView` may be reused by the table, so any additionally inserted views should be removed at this point.

## See Also

### Working with NSView-Based Outline Views

func outlineView(NSOutlineView, didAdd: NSTableRowView, forRow: Int)

Implemented to know when a new row view is added to the table.

func outlineView(NSOutlineView, rowViewForItem: Any) -> NSTableRowView?

implement this method to return a custom `NSTableRowView` for a particular item.

func outlineView(NSOutlineView, viewFor: NSTableColumn?, item: Any) -> NSView?

Implemented to return the view used to display the specified item and column.

