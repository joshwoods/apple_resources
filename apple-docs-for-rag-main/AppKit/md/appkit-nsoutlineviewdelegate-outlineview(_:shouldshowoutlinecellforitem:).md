

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:shouldShowOutlineCellForItem:) 

Instance Method

# outlineView(\_:shouldShowOutlineCellForItem:)

Returns whether the specified item should display the outline cell (the disclosure triangle).

macOS 10.6+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    shouldShowOutlineCellForItem item: Any
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`item`  

An item in the outline view.

## Return Value

true if the outline cell should be displayed, otherwise false.

## Discussion

Returning false causes frameOfOutlineCell(atRow:) to return `NSZeroRect`, hiding the cell. In addition, the row will not be collapsible by keyboard shortcuts.

This method is called only for expandable rows.

## See Also

### Displaying Cells

func outlineView(NSOutlineView, willDisplayCell: Any, for: NSTableColumn?, item: Any)

Informs the delegate that the cell specified by the column and item will be displayed.

func outlineView(NSOutlineView, willDisplayOutlineCell: Any, for: NSTableColumn?, item: Any)

Informs the delegate that an outline view is about to display a cell used to draw the expansion symbol.

func outlineView(NSOutlineView, dataCellFor: NSTableColumn?, item: Any) -> NSCell?

Returns the cell to use in a given column for a given item.

func outlineView(NSOutlineView, shouldShowCellExpansionFor: NSTableColumn?, item: Any) -> Bool

Invoked to allow the delegate to control cell expansion for a specific column and item.

