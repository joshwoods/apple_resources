

- AppKit
- View Management
- NSSplitViewController
-  Protocol Implementations 

API Collection

# Protocol Implementations

Access the split view controller’s implementations of protocol methods.

## Overview

NSSplitViewController conforms to NSSplitViewDelegate to serve as its split view’s delegate. This page lists the split view controller type’s implementations of those protocol methods. If you override these methods in a subclass, you must call `super`.

NSSplitViewController also conforms to NSUserInterfaceValidations by implementing validateUserInterfaceItem(_:).

## Topics

### Configuring and Drawing View Dividers

func splitView(NSSplitView, effectiveRect: NSRect, forDrawnRect: NSRect, ofDividerAt: Int) -> NSRect

Allows the split view controller to modify the rectangle where mouse clicks initiate divider dragging.

func splitView(NSSplitView, shouldHideDividerAt: Int) -> Bool

Allows the split view controller to determine whether the user can drag a divider or adjust it off the edge of the split view.

func splitView(NSSplitView, additionalEffectiveRectOfDividerAt: Int) -> NSRect

Allows the split view controller to return an additional rectangle where mouse clicks can initiate divider dragging.

### Managing Subviews

func splitView(NSSplitView, canCollapseSubview: NSView) -> Bool

Allows the split view controller to determine whether the user can collapse and expand the specified subview.

func splitView(NSSplitView, shouldCollapseSubview: NSView, forDoubleClickOnDividerAt: Int) -> Bool

Allows the split view controller to determine if a subview collapses in response to a double click.

Deprecated

### Validating User Interface Items

func validateUserInterfaceItem(any NSValidatedUserInterfaceItem) -> Bool

Returns a Boolean value that indicates whether to enable the specified item.

