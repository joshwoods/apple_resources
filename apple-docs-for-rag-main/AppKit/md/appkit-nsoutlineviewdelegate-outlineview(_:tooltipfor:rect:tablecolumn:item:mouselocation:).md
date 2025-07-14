

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:toolTipFor:rect:tableColumn:item:mouseLocation:) 

Instance Method

# outlineView(\_:toolTipFor:rect:tableColumn:item:mouseLocation:)

When the cursor pauses over a given cell, the value returned from this method is displayed in a tooltip.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    toolTipFor cell: NSCell,
    rect: NSRectPointer,
    tableColumn: NSTableColumn?,
    item: Any,
    mouseLocation: NSPoint
) -> String
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`cell`  

The cell for which to generate a tooltip.

`rect`  

The proposed active area of the tooltip. To control the default active area, you can modify the `rect` parameter. By default, `rect` is computed as `[cell drawingRectForBounds:cellFrame]`.

`tableColumn`  

The table column that contains `cell`.

`item`  

The item for which to display a tooltip.

`mouseLocation`  

The current mouse location in view coordinates.

## Return Value

If you don’t want a tooltip at that location, return an empty string.

