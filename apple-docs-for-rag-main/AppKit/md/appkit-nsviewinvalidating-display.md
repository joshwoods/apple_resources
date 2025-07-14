

- AppKit
- NSViewInvalidating
-  display 

Type Property

# display

A change that requires the system to redraw a view’s content.

macOS 12.0+Swift 5.1+

``` source
static var display: NSView.Invalidations.Display { get }
```

Available when `Self` is `NSView.Invalidations.Display`.

## Discussion

Use this invalidation type to set needsDisplay so that a change in property value triggers the system to redraw the containing view’s content.

## See Also

### Types of Invalidations

static var constraints: NSView.Invalidations.Constraints

A change that invalidates a view’s constraints.

static var intrinsicContentSize: NSView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

static var layout: NSView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

static var restorableState: NSView.Invalidations.RestorableState

A change that invalidates the restorable state of the view.

