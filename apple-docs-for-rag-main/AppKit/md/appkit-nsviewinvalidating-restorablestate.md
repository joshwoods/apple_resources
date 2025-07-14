

- AppKit
- NSViewInvalidating
-  restorableState 

Type Property

# restorableState

A change that invalidates the restorable state of the view.

macOS 12.0+Swift 5.1+

``` source
static var restorableState: NSView.Invalidations.RestorableState { get }
```

Available when `Self` is `NSView.Invalidations.RestorableState`.

## Discussion

Use this invalidation type to call invalidateRestorableState() so that a change in property value invalidates the viewʼs restorable state. This triggers the app to save any information the restoration system needs to restore the current state of the view.

## See Also

### Types of Invalidations

static var constraints: NSView.Invalidations.Constraints

A change that invalidates a view’s constraints.

static var display: NSView.Invalidations.Display

A change that requires the system to redraw a view’s content.

static var intrinsicContentSize: NSView.Invalidations.IntrinsicContentSize

A change that invalidates a view’s intrinsic size.

static var layout: NSView.Invalidations.Layout

A change that invalidates the layout of the containing view’s subviews.

