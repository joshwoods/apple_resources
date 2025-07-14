

- UIKit
- UIView
-  rightAnchor 

Instance Property

# rightAnchor

A layout anchor representing the right edge of the view’s frame.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var rightAnchor: NSLayoutXAxisAnchor { get }
```

## Discussion

Use this anchor to create constraints with the view’s right edge. You can combine this anchor only with a subset of the NSLayoutXAxisAnchor anchors. You can combine a UIView with another `rightAnchor`, a `leftAnchor`, or a `centerXAnchor`. For more information, see NSLayoutAnchor.

## See Also

### Creating constraints using layout anchors

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

var topAnchor: NSLayoutYAxisAnchor

A layout anchor representing the top edge of the view’s frame.

var trailingAnchor: NSLayoutXAxisAnchor

A layout anchor representing the trailing edge of the view’s frame.

var widthAnchor: NSLayoutDimension

A layout anchor representing the width of the view’s frame.

