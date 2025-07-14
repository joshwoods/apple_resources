

- AppKit
-  NSViewInvalidating 

Protocol

# NSViewInvalidating

Implements a type of invalidation that can occur on a view that requires an update.

macOS 12.0+Swift 5.1+

``` source
protocol NSViewInvalidating
```

## Topics

### Types of Invalidations

static var constraints: NSView.Invalidations.Constraints

A change that invalidates a view’s constraints.

static var display: NSView.Invalidations.Display

A change that requires the system to redraw a view’s content.

static var intrinsicContentSize: NSView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

static var layout: NSView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

static var restorableState: NSView.Invalidations.RestorableState

A change that invalidates the restorable state of the view.

### Supporting Types

func invalidate(view: NSView)

Indicates to the system that an aspect of a view is invalid and triggers the necessary update.

**Required**

enum Invalidations

Changes that cause aspects of a view to be invalid and require an update.

## Relationships

### Conforming Types

- NSView.Invalidations.Constraints
- NSView.Invalidations.Display
- NSView.Invalidations.IntrinsicContentSize
- NSView.Invalidations.Layout
- NSView.Invalidations.RestorableState
- NSView.Invalidations.Tuple

## See Also

### Updating the View When Property Values Change

struct Invalidating

A property wrapper that notifies the system that a property value change has invalidated an aspect of the containing view.

