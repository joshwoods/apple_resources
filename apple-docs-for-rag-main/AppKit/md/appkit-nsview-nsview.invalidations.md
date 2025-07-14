

- AppKit
- NSView
-  NSView.Invalidations 

Enumeration

# NSView.Invalidations

Changes that cause aspects of a view to be invalid and require an update.

macOS 12.0+Swift 5.1+

``` source
enum Invalidations
```

## Topics

### Types of Invalidations

struct Constraints

A change that invalidates a view’s constraints.

struct Display

A change that requires the system to redraw a view’s content.

struct IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

struct Layout

A change that invalidates the layout of the containing view’s subviews.

struct RestorableState

A change that invalidates the restorable state of the view.

struct Tuple

A change that invalidates a combination of factors covered by the other invalidation types.

## See Also

### Supporting Types

func invalidate(view: NSView)

Indicates to the system that an aspect of a view is invalid and triggers the necessary update.

**Required**

