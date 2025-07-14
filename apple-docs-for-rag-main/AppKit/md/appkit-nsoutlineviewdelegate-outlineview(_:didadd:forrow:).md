

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:didAdd:forRow:) 

Instance Method

# outlineView(\_:didAdd:forRow:)

Implemented to know when a new row view is added to the table.

macOS 10.7+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    didAdd rowView: NSTableRowView,
    forRow row: Int
)
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`rowView`  

The new row view.

`row`  

The row to which the view was added.

## Discussion

This delegate method is for NSView-based outline views. At this point, you can choose to add in extra views or modify any properties on `rowView`.

## See Also

### Working with NSView-Based Outline Views

func outlineView(NSOutlineView, didRemove: NSTableRowView, forRow: Int)

Implemented to know when a row view is removed from the table

func outlineView(NSOutlineView, rowViewForItem: Any) -> NSTableRowView?

implement this method to return a custom `NSTableRowView` for a particular item.

func outlineView(NSOutlineView, viewFor: NSTableColumn?, item: Any) -> NSView?

Implemented to return the view used to display the specified item and column.

