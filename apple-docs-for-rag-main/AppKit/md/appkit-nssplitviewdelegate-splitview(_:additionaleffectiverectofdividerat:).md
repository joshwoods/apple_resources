

- AppKit
- NSSplitViewDelegate
-  splitView(\_:additionalEffectiveRectOfDividerAt:) 

Instance Method

# splitView(\_:additionalEffectiveRectOfDividerAt:)

Allows the delegate to return an additional rectangle where mouse clicks can initiate divider dragging.

macOS 10.5+

``` source
@MainActor
optional func splitView(
    _ splitView: NSSplitView,
    additionalEffectiveRectOfDividerAt dividerIndex: Int
) -> NSRect
```

## Parameters 

`splitView`  

The split view that sends the message.

`dividerIndex`  

The index of the divider.

## Return Value

An additional rectangle, in the coordinate system that `splitView` defines, where mouse clicks can initiate divider dragging. Returning NSZeroRect indicates no additional dragging rectangle is necessary.

## Discussion

If a split view has no delegate, or if its delegate doesn’t respond to this message, only mouse clicks within the effective frame of a divider initiate divider dragging.

## See Also

### Configuring and Drawing View Dividers

func splitView(NSSplitView, effectiveRect: NSRect, forDrawnRect: NSRect, ofDividerAt: Int) -> NSRect

Allows the delegate to modify the rectangle where mouse clicks initiate divider dragging.

func splitView(NSSplitView, shouldHideDividerAt: Int) -> Bool

Allows the delegate to determine whether the user can drag a divider or adjust it off the edge of the split view.

