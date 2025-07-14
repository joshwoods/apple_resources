

- AppKit
- NSSplitViewDelegate
-  splitView(\_:shouldHideDividerAt:) 

Instance Method

# splitView(\_:shouldHideDividerAt:)

Allows the delegate to determine whether the user can drag a divider or adjust it off the edge of the split view.

macOS 10.5+

``` source
@MainActor
optional func splitView(
    _ splitView: NSSplitView,
    shouldHideDividerAt dividerIndex: Int
) -> Bool
```

## Parameters 

`splitView`  

The split view that sends the message.

`dividerIndex`  

The zero-based index of the divider.

## Return Value

true if the user can drag the divider off the edge of the split view, resulting in it not being visible.

## Discussion

If a split view has no delegate, or if its delegate doesn’t respond to this message, the split view behaves as if it has a delegate that returns false when it receives this message.

## See Also

### Configuring and Drawing View Dividers

func splitView(NSSplitView, effectiveRect: NSRect, forDrawnRect: NSRect, ofDividerAt: Int) -> NSRect

Allows the delegate to modify the rectangle where mouse clicks initiate divider dragging.

func splitView(NSSplitView, additionalEffectiveRectOfDividerAt: Int) -> NSRect

Allows the delegate to return an additional rectangle where mouse clicks can initiate divider dragging.

