

- AppKit
- NSSplitViewController
-  splitView(\_:shouldHideDividerAt:) 

Instance Method

# splitView(\_:shouldHideDividerAt:)

Allows the split view controller to determine whether the user can drag a divider or adjust it off the edge of the split view.

macOS 10.10+

``` source
@MainActor
func splitView(
    _ splitView: NSSplitView,
    shouldHideDividerAt dividerIndex: Int
) -> Bool
```

## Discussion

By default, NSSplitViewController hides the first and last dividers if their outer neighbor is in a collapsed state.

## See Also

### Configuring and Drawing View Dividers

func splitView(NSSplitView, effectiveRect: NSRect, forDrawnRect: NSRect, ofDividerAt: Int) -> NSRect

Allows the split view controller to modify the rectangle where mouse clicks initiate divider dragging.

func splitView(NSSplitView, additionalEffectiveRectOfDividerAt: Int) -> NSRect

Allows the split view controller to return an additional rectangle where mouse clicks can initiate divider dragging.

