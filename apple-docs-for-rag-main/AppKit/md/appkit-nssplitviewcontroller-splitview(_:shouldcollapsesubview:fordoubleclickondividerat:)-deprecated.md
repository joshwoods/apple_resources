

- AppKit
- NSSplitViewController
-  splitView(\_:shouldCollapseSubview:forDoubleClickOnDividerAt:) Deprecated

Instance Method

# splitView(\_:shouldCollapseSubview:forDoubleClickOnDividerAt:)

Allows the split view controller to determine if a subview collapses in response to a double click.

macOS 10.5–10.15Deprecated

``` source
@MainActor
func splitView(
    _ splitView: NSSplitView,
    shouldCollapseSubview subview: NSView,
    forDoubleClickOnDividerAt dividerIndex: Int
) -> Bool
```

Deprecated

NSSplitView no longer supports collapsing sections using a double click. The system never calls this delegate method, and this implementation always returns false.

## See Also

### Managing Subviews

func splitView(NSSplitView, canCollapseSubview: NSView) -> Bool

Allows the split view controller to determine whether the user can collapse and expand the specified subview.

