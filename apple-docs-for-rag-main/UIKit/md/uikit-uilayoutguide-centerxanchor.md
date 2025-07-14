

- UIKit
- UILayoutGuide
-  centerXAnchor 

Instance Property

# centerXAnchor

A layout anchor representing the horizontal center of the layout guide’s frame.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var centerXAnchor: NSLayoutXAxisAnchor { get }
```

## Discussion

Use this anchor to create constraints with the layout guide’s horizontal center. You can combine this anchor only with other NSLayoutXAxisAnchor anchors. For more information, see NSLayoutAnchor.

## See Also

### Creating constraints using layout anchors

var bottomAnchor: NSLayoutYAxisAnchor

A layout anchor representing the bottom edge of the layout guide’s frame.

var centerYAnchor: NSLayoutYAxisAnchor

A layout anchor representing the vertical center of the layout guide’s frame.

var heightAnchor: NSLayoutDimension

A layout anchor representing the height of the layout guide’s frame.

var leadingAnchor: NSLayoutXAxisAnchor

A layout anchor representing the leading edge of the layout guide’s frame.

var leftAnchor: NSLayoutXAxisAnchor

A layout anchor representing the left edge of the layout guide’s frame.

var rightAnchor: NSLayoutXAxisAnchor

A layout anchor representing the right edge of the layout guide’s frame.

var topAnchor: NSLayoutYAxisAnchor

A layout anchor representing the top edge of the layout guide’s frame.

var trailingAnchor: NSLayoutXAxisAnchor

A layout anchor representing the trailing edge of the layout guide’s frame.

var widthAnchor: NSLayoutDimension

A layout anchor representing the width of the layout guide’s frame.

