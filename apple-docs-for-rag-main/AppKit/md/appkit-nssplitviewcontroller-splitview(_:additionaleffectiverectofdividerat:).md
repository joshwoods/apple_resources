

- AppKit
- NSSplitViewController
-  splitView(\_:additionalEffectiveRectOfDividerAt:) 

Instance Method

# splitView(\_:additionalEffectiveRectOfDividerAt:)

Allows the split view controller to return an additional rectangle where mouse clicks can initiate divider dragging.

macOS 10.10+

``` source
@MainActor
func splitView(
    _ splitView: NSSplitView,
    additionalEffectiveRectOfDividerAt dividerIndex: Int
) -> NSRect
```

## See Also

### Configuring and Drawing View Dividers

func splitView(NSSplitView, effectiveRect: NSRect, forDrawnRect: NSRect, ofDividerAt: Int) -> NSRect

Allows the split view controller to modify the rectangle where mouse clicks initiate divider dragging.

func splitView(NSSplitView, shouldHideDividerAt: Int) -> Bool

Allows the split view controller to determine whether the user can drag a divider or adjust it off the edge of the split view.

