

- AppKit
- NSView
-  resize(withOldSuperviewSize:) 

Instance Method

# resize(withOldSuperviewSize:)

Informs the view that the bounds size of its superview has changed.

macOS

``` source
@MainActor
func resize(withOldSuperviewSize oldSize: NSSize)
```

## Parameters 

`oldSize`  

The previous size of the superview’s bounds rectangle.

## Discussion

This method is normally invoked automatically from resizeSubviews(withOldSize:).

The default implementation resizes the view according to the autoresizing options specified by the autoresizingMask property. You shouldn’t invoke this method directly, but you can override it to define a specific resizing behavior.

If you override this method and call `super` as part of your implementation, you should be sure to call `super` before making changes to the receiving view’s frame yourself.

## See Also

### Resizing Subviews

var autoresizesSubviews: Bool

A Boolean value indicating whether the view applies the autoresizing behavior to its subviews when its frame size changes.

var autoresizingMask: NSView.AutoresizingMask

The options that determine how the view is resized relative to its superview.

struct AutoresizingMask

Constants that specify the autoresizing behaviors for views.

func resizeSubviews(withOldSize: NSSize)

Informs the view’s subviews that the view’s bounds rectangle size has changed.

