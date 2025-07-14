

- AppKit
- NSView
-  autoresizesSubviews 

Instance Property

# autoresizesSubviews

A Boolean value indicating whether the view applies the autoresizing behavior to its subviews when its frame size changes.

macOS

``` source
@MainActor
var autoresizesSubviews: Bool { get set }
```

## Discussion

When the value of this property is true and the view’s frame changes, the view automatically calls the resizeSubviews(withOldSize:) method to facilitate the resizing of its subviews. When the value of this property is false, the view does not autoresize its subviews.

The default value of this property is true.

## See Also

### Resizing Subviews

var autoresizingMask: NSView.AutoresizingMask

The options that determine how the view is resized relative to its superview.

struct AutoresizingMask

Constants that specify the autoresizing behaviors for views.

func resizeSubviews(withOldSize: NSSize)

Informs the view’s subviews that the view’s bounds rectangle size has changed.

func resize(withOldSuperviewSize: NSSize)

Informs the view that the bounds size of its superview has changed.

