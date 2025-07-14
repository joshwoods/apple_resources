

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:didDrag:) 

Instance Method

# outlineView(\_:didDrag:)

Sent at the time the mouse button goes up in `outlineView` and `tableColumn` has been dragged during the time the mouse button was down.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    didDrag tableColumn: NSTableColumn
)
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`tableColumn`  

The table column.

## See Also

### Working with Table Columns

func outlineView(NSOutlineView, mouseDownInHeaderOf: NSTableColumn)

Sent to the delegate whenever the mouse button is clicked in `outlineView` while the cursor is in a column header `tableColumn`.

func outlineView(NSOutlineView, didClick: NSTableColumn)

Sent at the time the mouse button subsequently goes up in `outlineView` and `tableColumn` has been “clicked” without having been dragged anywhere.

