

- AppKit
- NSScrollView
-  maxMagnification 

Instance Property

# maxMagnification

The maximum value to which the content can be magnified.

macOS 10.8+

``` source
@MainActor
var maxMagnification: CGFloat { get set }
```

## Discussion

This value must be greater than or equal to the minimum magnification. The default value is `4.0`.

## See Also

### Zooming the Scroll View

var allowsMagnification: Bool

Allows the user to magnify the scroll view.

var magnification: CGFloat

The amount by which the content is currently scaled.

func magnify(toFit: NSRect)

Magnifies the content view proportionally such that the given rectangle fits centered in the scroll view.

var minMagnification: CGFloat

The minimum value to which the content can be magnified.

func setMagnification(CGFloat, centeredAt: NSPoint)

Magnify the content by the given amount and center the result on the given point.

