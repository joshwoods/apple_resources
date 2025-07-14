

- AppKit
- NSSplitViewDelegate
-  splitView(\_:shouldCollapseSubview:forDoubleClickOnDividerAt:) Deprecated

Instance Method

# splitView(\_:shouldCollapseSubview:forDoubleClickOnDividerAt:)

Allows a delegate to determine if a subview collapses in response to a double click.

macOS 10.5–10.15Deprecated

``` source
optional func splitView(
    _ splitView: NSSplitView,
    shouldCollapseSubview subview: NSView,
    forDoubleClickOnDividerAt dividerIndex: Int
) -> Bool
```

Deprecated

NSSplitView no longer supports collapsing sections via double-click. This delegate method is never called.

## Parameters 

`splitView`  

The split view that sends the message.

`subview`  

The subview to collapse.

`dividerIndex`  

The index of the divider.

## Return Value

true if the subview should collapse; otherwise, false.

## Discussion

If the delegate implements this method, it receives this message once for the subview before a divider when the user double-clicks that divider, and again for the subview after the divider, but only if the delegate returns true when it receives splitView(_:canCollapseSubview:) for the subview in question. When the delegate indicates that both subviews should collapse, the behavior of NSSplitView is undefined.

## See Also

### Managing Subviews

func splitViewWillResizeSubviews(Notification)

Notifies the delegate when the split view is about to resize its subviews.

func splitViewDidResizeSubviews(Notification)

Notifies the delegate when the split view resizes its subviews.

func splitView(NSSplitView, canCollapseSubview: NSView) -> Bool

Allows the delegate to determine whether the user can collapse and expand the specified subview.

