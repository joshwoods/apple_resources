

- AppKit
- NSSplitViewDelegate
-  splitViewWillResizeSubviews(\_:) 

Instance Method

# splitViewWillResizeSubviews(\_:)

Notifies the delegate when the split view is about to resize its subviews.

macOS 10.10+

``` source
@MainActor
optional func splitViewWillResizeSubviews(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willResizeSubviewsNotification, which posts before a change to the size of some or all subviews of a split view.

## Discussion

If the delegate implements this method, the system automatically registers it to receive this notification.

The default notification center invokes this method before the split view resizes two of its subviews in response to the repositioning of a divider.

## See Also

### Managing Subviews

func splitViewDidResizeSubviews(Notification)

Notifies the delegate when the split view resizes its subviews.

func splitView(NSSplitView, canCollapseSubview: NSView) -> Bool

Allows the delegate to determine whether the user can collapse and expand the specified subview.

func splitView(NSSplitView, shouldCollapseSubview: NSView, forDoubleClickOnDividerAt: Int) -> Bool

Allows a delegate to determine if a subview collapses in response to a double click.

Deprecated

