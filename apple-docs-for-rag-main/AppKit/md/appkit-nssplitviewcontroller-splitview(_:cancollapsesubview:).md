

- AppKit
- NSSplitViewController
-  splitView(\_:canCollapseSubview:) 

Instance Method

# splitView(\_:canCollapseSubview:)

Allows the split view controller to determine whether the user can collapse and expand the specified subview.

macOS 10.10+

``` source
@MainActor
func splitView(
    _ splitView: NSSplitView,
    canCollapseSubview subview: NSView
) -> Bool
```

## See Also

### Managing Subviews

func splitView(NSSplitView, shouldCollapseSubview: NSView, forDoubleClickOnDividerAt: Int) -> Bool

Allows the split view controller to determine if a subview collapses in response to a double click.

Deprecated

