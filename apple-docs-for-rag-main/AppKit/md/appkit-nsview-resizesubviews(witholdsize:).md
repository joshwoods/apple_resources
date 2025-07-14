

- AppKit
- NSView
-  resizeSubviews(withOldSize:) 

Instance Method

# resizeSubviews(withOldSize:)

Informs the view’s subviews that the view’s bounds rectangle size has changed.

macOS

``` source
@MainActor
func resizeSubviews(withOldSize oldSize: NSSize)
```

## Parameters 

`oldSize`  

The previous size of the view’s bounds rectangle.

## Discussion

If the view is configured to autoresize its subviews, this method is automatically invoked by any method that changes the view’s frame size.

The default implementation sends resize(withOldSuperviewSize:) to the view’s subviews with `oldBoundsSize` as the argument. You shouldn’t invoke this method directly, but you can override it to define a specific resizing behavior.

## See Also

### Resizing Subviews

var autoresizesSubviews: Bool

A Boolean value indicating whether the view applies the autoresizing behavior to its subviews when its frame size changes.

var autoresizingMask: NSView.AutoresizingMask

The options that determine how the view is resized relative to its superview.

struct AutoresizingMask

Constants that specify the autoresizing behaviors for views.

func resize(withOldSuperviewSize: NSSize)

Informs the view that the bounds size of its superview has changed.

