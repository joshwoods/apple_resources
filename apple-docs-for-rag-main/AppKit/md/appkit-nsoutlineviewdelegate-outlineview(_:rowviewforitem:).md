

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:rowViewForItem:) 

Instance Method

# outlineView(\_:rowViewForItem:)

implement this method to return a custom `NSTableRowView` for a particular item.

macOS 10.7+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    rowViewForItem item: Any
) -> NSTableRowView?
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`item`  

The item displayed by the returned table row view.

## Return Value

An instance or subclass of `NSTableRowView`. If `nil` is returned, a `NSTableRowView` instance is created and used.

## Discussion

This method, if implemented, is only invoked for NSView-based outline views.

## See Also

### Working with NSView-Based Outline Views

func outlineView(NSOutlineView, didAdd: NSTableRowView, forRow: Int)

Implemented to know when a new row view is added to the table.

func outlineView(NSOutlineView, didRemove: NSTableRowView, forRow: Int)

Implemented to know when a row view is removed from the table

func outlineView(NSOutlineView, viewFor: NSTableColumn?, item: Any) -> NSView?

Implemented to return the view used to display the specified item and column.

