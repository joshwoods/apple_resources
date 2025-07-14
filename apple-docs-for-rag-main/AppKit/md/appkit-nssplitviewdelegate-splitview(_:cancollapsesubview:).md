

- AppKit
- NSSplitViewDelegate
-  splitView(\_:canCollapseSubview:) 

Instance Method

# splitView(\_:canCollapseSubview:)

Allows the delegate to determine whether the user can collapse and expand the specified subview.

macOS

``` source
@MainActor
optional func splitView(
    _ splitView: NSSplitView,
    canCollapseSubview subview: NSView
) -> Bool
```

## Parameters 

`splitView`  

The split view that sends the message.

`subview`  

The subview to collapse.

## Return Value

true if `subview` collapses when the user drags a divider beyond the halfway mark between its minimum size and its edge; otherwise, false.

## Discussion

The `subview` expands when the user drags the divider beyond the halfway mark between its minimum size and its edge.

To specify the minimum size, define the methods splitView(_:constrainMaxCoordinate:ofSubviewAt:) and splitView(_:constrainMinCoordinate:ofSubviewAt:). A subview can collapse only if you also define splitView(_:constrainMinCoordinate:ofSubviewAt:).

A collapsed subview isn’t visible, but the split view object retains it with the same size as before the collapse.

If the delegate doesn’t implement this method, the subviews can’t collapse.

## See Also

### Managing Subviews

func splitViewWillResizeSubviews(Notification)

Notifies the delegate when the split view is about to resize its subviews.

func splitViewDidResizeSubviews(Notification)

Notifies the delegate when the split view resizes its subviews.

func splitView(NSSplitView, shouldCollapseSubview: NSView, forDoubleClickOnDividerAt: Int) -> Bool

Allows a delegate to determine if a subview collapses in response to a double click.

Deprecated

