

- AppKit
- NSScrollView
-  magnification 

Instance Property

# magnification

The amount by which the content is currently scaled.

macOS 10.8+

``` source
@MainActor
var magnification: CGFloat { get set }
```

## Discussion

To animate the magnification, use the object’s animator. The default value is `1.0`.

## See Also

### Zooming the Scroll View

var allowsMagnification: Bool

Allows the user to magnify the scroll view.

func magnify(toFit: NSRect)

Magnifies the content view proportionally such that the given rectangle fits centered in the scroll view.

var maxMagnification: CGFloat

The maximum value to which the content can be magnified.

var minMagnification: CGFloat

The minimum value to which the content can be magnified.

func setMagnification(CGFloat, centeredAt: NSPoint)

Magnify the content by the given amount and center the result on the given point.

