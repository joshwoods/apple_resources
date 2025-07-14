

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:shouldTrackCell:for:item:) 

Instance Method

# outlineView(\_:shouldTrackCell:for:item:)

Returns a Boolean value that indicates whether a given cell should be tracked.

macOS 10.5+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    shouldTrackCell cell: NSCell,
    for tableColumn: NSTableColumn?,
    item: Any
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`cell`  

The cell used to display item `item` in column `tableColumn`

`tableColumn`  

A table column in the outline view.

`item`  

An item in the outline view.

## Return Value

true if the cell should be tracked for the item `item` in column `tableColumn`, otherwise false.

## Discussion

Normally, only selectable or selected cells can be tracked. If you implement this method, cells which are not selectable or selected can be tracked (and vice-versa). For example, this allows you to have a button cell in a table which does not change the selection, but can still be clicked on and tracked.

