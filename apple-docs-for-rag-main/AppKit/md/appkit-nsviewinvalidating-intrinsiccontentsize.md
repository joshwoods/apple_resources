

- AppKit
- NSViewInvalidating
-  intrinsicContentSize 

Type Property

# intrinsicContentSize

A change that invalidates a view’s intrinsic size.

macOS 12.0+Swift 5.1+

``` source
static var intrinsicContentSize: NSView.Invalidations.IntrinsicContentSize { get }
```

Available when `Self` is `NSView.Invalidations.IntrinsicContentSize`.

## Discussion

Use this invalidation type to call invalidateIntrinsicContentSize() so that a change in property value invalidates the containing view’s intrinsic content size. This allows the constraint-based layout system to account for the change the next time it updates the layout.

## See Also

### Types of Invalidations

static var constraints: NSView.Invalidations.Constraints

A change that invalidates a view’s constraints.

static var display: NSView.Invalidations.Display

A change that requires the system to redraw a view’s content.

static var layout: NSView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

static var restorableState: NSView.Invalidations.RestorableState

A change that invalidates the restorable state of the view.

