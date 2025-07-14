

- AppKit
-  NSSplitView 

Class

# NSSplitView

A view that arranges two or more views in a linear stack running horizontally or vertically.

macOS

``` source
@MainActor
class NSSplitView
```

## Overview

A split view manages the dividers and orientation for a split view controller (NSSplitViewController). By default, dividers have a horizontal orientation so that the split view arranges its panes vertically from top to bottom.

Divider indices are zero-based. If the isVertical property is false, which is the default value, the top divider has an index of `0`. If isVertical is true, the leading divider has an index of `0`.

## Topics

### Customizing the Split View Behavior

var delegate: (any NSSplitViewDelegate)?

The split view’s delegate.

protocol NSSplitViewDelegate

A set of optional methods that a delegate of a split view implements.

### Arranging Subviews

var arrangesAllSubviews: Bool

A Boolean value that determines whether the split view arranges all of its subviews as split panes.

var arrangedSubviews: [NSView]

The array of views that the split view arranges as its split panes.

func addArrangedSubview(NSView)

Adds a view as an arranged split pane.

func insertArrangedSubview(NSView, at: Int)

Adds a view as an arranged split pane at the specified index.

func removeArrangedSubview(NSView)

Removes a view as an arranged split pane.

### Managing Subviews

func adjustSubviews()

Adjusts the sizes of the split view’s subviews so they (plus the dividers) fill the split view.

func isSubviewCollapsed(NSView) -> Bool

Returns whether the specified view is in a collapsed state.

func holdingPriorityForSubview(at: Int) -> NSLayoutConstraint.Priority

Returns the priority of the subview’s width or height when resizing.

func setHoldingPriority(NSLayoutConstraint.Priority, forSubviewAt: Int)

Sets the priority for split view subviews to maintain their width or height.

### Managing Divider Orientation

var isVertical: Bool

A Boolean value that determines the geometric orientation of the split view’s dividers.

### Configuring and Drawing Dividers

var dividerStyle: NSSplitView.DividerStyle

The style of divider between views.

enum DividerStyle

Constants that specify the style of the split view’s dividers.

var dividerColor: NSColor

The color of the dividers that the split view draws between subviews.

var dividerThickness: CGFloat

The thickness of the dividers for the split view.

func drawDivider(in: NSRect)

Draws a divider between two of the split view’s subviews.

### Saving Subview Positions

var autosaveName: NSSplitView.AutosaveName?

The name to use when the system automatically saves the split view’s divider configuration.

typealias AutosaveName

The type that specifies the split view’s autosave name.

### Constraining Split Position

func minPossiblePositionOfDivider(at: Int) -> CGFloat

Returns the minimum possible position of the divider at the specified index.

func maxPossiblePositionOfDivider(at: Int) -> CGFloat

Returns the maximum possible position of the divider at the specified index.

func setPosition(CGFloat, ofDividerAt: Int)

Updates the location of a divider you specify by index.

### Managing Notifications

class let willResizeSubviewsNotification: NSNotification.Name

A notification that posts before a change to the size of some or all subviews of a split view.

class let didResizeSubviewsNotification: NSNotification.Name

A notification that posts after a change to the size of some or all subviews of a split view.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Split View Interface

class NSSplitViewController

An object that manages an array of adjacent child views, and has a split view object for managing dividers between those views.

class NSSplitViewItem

An item in a split view controller.

