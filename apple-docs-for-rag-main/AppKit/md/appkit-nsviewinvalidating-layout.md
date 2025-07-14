

- AppKit
- NSViewInvalidating
-  layout 

Type Property

# layout

A change that invalidates the layout of the containing view’s subviews.

macOS 12.0+Swift 5.1+

``` source
static var layout: NSView.Invalidations.Layout { get }
```

Available when `Self` is `NSView.Invalidations.Layout`.

## Discussion

Use this invalidation type to set needsLayout so that a change in property value triggers the system to update the layout of the containing view’s subviews.

## See Also

### Types of Invalidations

static var constraints: NSView.Invalidations.Constraints

A change that invalidates a view’s constraints.

static var display: NSView.Invalidations.Display

A change that requires the system to redraw a view’s content.

static var intrinsicContentSize: NSView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

static var restorableState: NSView.Invalidations.RestorableState

A change that invalidates the restorable state of the view.

