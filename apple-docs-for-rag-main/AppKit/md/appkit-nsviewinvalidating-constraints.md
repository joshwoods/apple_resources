

- AppKit
- NSViewInvalidating
-  constraints 

Type Property

# constraints

A change that invalidates a view’s constraints.

macOS 12.0+Swift 5.1+

``` source
static var constraints: NSView.Invalidations.Constraints { get }
```

Available when `Self` is `NSView.Invalidations.Constraints`.

## Discussion

Use this invalidation type to set needsUpdateConstraints so that a change in property value triggers the containing view to update constraints.

## See Also

### Types of Invalidations

static var display: NSView.Invalidations.Display

A change that requires the system to redraw a view’s content.

static var intrinsicContentSize: NSView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

static var layout: NSView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

static var restorableState: NSView.Invalidations.RestorableState

A change that invalidates the restorable state of the view.

