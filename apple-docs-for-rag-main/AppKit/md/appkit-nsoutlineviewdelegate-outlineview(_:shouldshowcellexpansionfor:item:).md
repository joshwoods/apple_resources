

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:shouldShowCellExpansionFor:item:) 

Instance Method

# outlineView(\_:shouldShowCellExpansionFor:item:)

Invoked to allow the delegate to control cell expansion for a specific column and item.

macOS 10.5+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    shouldShowCellExpansionFor tableColumn: NSTableColumn?,
    item: Any
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`tableColumn`  

A table column in the outline view.

`item`  

An item in the outline view.

## Return Value

true to allow an expansion tooltip to appear in the column `tableColumn` for item `item`, otherwise false.

## Discussion

Cell expansion can occur when the mouse hovers over the specified cell and the cell contents are unable to be fully displayed within the cell. If this method returns true, the full cell contents will be shown in a special floating tool tip view, otherwise the content is truncated.

## See Also

### Displaying Cells

func outlineView(NSOutlineView, willDisplayCell: Any, for: NSTableColumn?, item: Any)

Informs the delegate that the cell specified by the column and item will be displayed.

func outlineView(NSOutlineView, willDisplayOutlineCell: Any, for: NSTableColumn?, item: Any)

Informs the delegate that an outline view is about to display a cell used to draw the expansion symbol.

func outlineView(NSOutlineView, dataCellFor: NSTableColumn?, item: Any) -> NSCell?

Returns the cell to use in a given column for a given item.

func outlineView(NSOutlineView, shouldShowOutlineCellForItem: Any) -> Bool

Returns whether the specified item should display the outline cell (the disclosure triangle).

