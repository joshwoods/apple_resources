

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:willDisplayCell:for:item:) 

Instance Method

# outlineView(\_:willDisplayCell:for:item:)

Informs the delegate that the cell specified by the column and item will be displayed.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    willDisplayCell cell: Any,
    for tableColumn: NSTableColumn?,
    item: Any
)
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`cell`  

The cell.

`tableColumn`  

The table column.

`item`  

The item.

## Discussion

The delegate can implement this method to modify `cell` to provide further setup for the `cell` in `tableColumn` and `item`. It is not safe to do drawing inside this method—you should only set up state for `cell`.

## See Also

### Displaying Cells

func outlineView(NSOutlineView, willDisplayOutlineCell: Any, for: NSTableColumn?, item: Any)

Informs the delegate that an outline view is about to display a cell used to draw the expansion symbol.

func outlineView(NSOutlineView, dataCellFor: NSTableColumn?, item: Any) -> NSCell?

Returns the cell to use in a given column for a given item.

func outlineView(NSOutlineView, shouldShowOutlineCellForItem: Any) -> Bool

Returns whether the specified item should display the outline cell (the disclosure triangle).

func outlineView(NSOutlineView, shouldShowCellExpansionFor: NSTableColumn?, item: Any) -> Bool

Invoked to allow the delegate to control cell expansion for a specific column and item.

