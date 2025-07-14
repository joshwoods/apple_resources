

- AppKit
-  NSSplitViewDelegate 

Protocol

# NSSplitViewDelegate

A set of optional methods that a delegate of a split view implements.

macOS

``` source
protocol NSSplitViewDelegate : NSObjectProtocol
```

## Topics

### Managing Subviews

func splitViewWillResizeSubviews(Notification)

Notifies the delegate when the split view is about to resize its subviews.

func splitViewDidResizeSubviews(Notification)

Notifies the delegate when the split view resizes its subviews.

func splitView(NSSplitView, canCollapseSubview: NSView) -> Bool

Allows the delegate to determine whether the user can collapse and expand the specified subview.

func splitView(NSSplitView, shouldCollapseSubview: NSView, forDoubleClickOnDividerAt: Int) -> Bool

Allows a delegate to determine if a subview collapses in response to a double click.

Deprecated

### Configuring and Drawing View Dividers

func splitView(NSSplitView, effectiveRect: NSRect, forDrawnRect: NSRect, ofDividerAt: Int) -> NSRect

Allows the delegate to modify the rectangle where mouse clicks initiate divider dragging.

func splitView(NSSplitView, shouldHideDividerAt: Int) -> Bool

Allows the delegate to determine whether the user can drag a divider or adjust it off the edge of the split view.

func splitView(NSSplitView, additionalEffectiveRectOfDividerAt: Int) -> NSRect

Allows the delegate to return an additional rectangle where mouse clicks can initiate divider dragging.

### Constraining Split Position

func splitView(NSSplitView, constrainSplitPosition: CGFloat, ofSubviewAt: Int) -> CGFloat

Allows the delegate to constrain the divider to certain positions.

### Adjusting Subviews Manually

func splitView(NSSplitView, constrainMinCoordinate: CGFloat, ofSubviewAt: Int) -> CGFloat

Allows the delegate to constrain the minimum coordinate limit of a divider when the user drags it.

func splitView(NSSplitView, constrainMaxCoordinate: CGFloat, ofSubviewAt: Int) -> CGFloat

Allows the delegate to constrain the maximum coordinate limit of a divider when the user drags it.

func splitView(NSSplitView, resizeSubviewsWithOldSize: NSSize)

Allows the delegate to specify custom sizing behavior for the subviews of the split view.

func splitView(NSSplitView, shouldAdjustSizeOfSubview: NSView) -> Bool

Allows the delegate to specify whether to resize the subview.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSSplitViewController

## See Also

### Customizing the Split View Behavior

var delegate: (any NSSplitViewDelegate)?

The split view’s delegate.

