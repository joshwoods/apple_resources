

- AppKit
- NSView
-  trailingAnchor 

Instance Property

# trailingAnchor

A layout anchor representing the trailing edge of the view’s frame.

macOS 10.11+

``` source
@MainActor
var trailingAnchor: NSLayoutXAxisAnchor { get }
```

## Discussion

Use this anchor to create constraints with the view’s trailing edge. You can only combine this anchor with a subset of the NSLayoutXAxisAnchor anchors. You can combine a `trailingAnchor` with another `trailingAnchor`, a `leadingAnchor`, or a `centerXAnchor`. For more information, see NSLayoutAnchor.

## See Also

### Creating Constraints Using Layout Anchors

var bottomAnchor: NSLayoutYAxisAnchor

A layout anchor representing the bottom edge of the view’s frame.

var centerXAnchor: NSLayoutXAxisAnchor

A layout anchor representing the horizontal center of the view’s frame.

var centerYAnchor: NSLayoutYAxisAnchor

A layout anchor representing the vertical center of the view’s frame.

var firstBaselineAnchor: NSLayoutYAxisAnchor

A layout anchor representing the baseline for the topmost line of text in the view.

var heightAnchor: NSLayoutDimension

A layout anchor representing the height of the view’s frame.

var lastBaselineAnchor: NSLayoutYAxisAnchor

A layout anchor representing the baseline for the bottommost line of text in the view.

var leadingAnchor: NSLayoutXAxisAnchor

A layout anchor representing the leading edge of the view’s frame.

var leftAnchor: NSLayoutXAxisAnchor

A layout anchor representing the left edge of the view’s frame.

var rightAnchor: NSLayoutXAxisAnchor

A layout anchor representing the right edge of the view’s frame.

var topAnchor: NSLayoutYAxisAnchor

A layout anchor representing the top edge of the view’s frame.

var widthAnchor: NSLayoutDimension

A layout anchor representing the width of the view’s frame.

