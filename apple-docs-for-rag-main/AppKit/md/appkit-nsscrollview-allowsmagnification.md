

- AppKit
- NSScrollView
-  allowsMagnification 

Instance Property

# allowsMagnification

Allows the user to magnify the scroll view.

macOS 10.8+

``` source
@MainActor
var allowsMagnification: Bool { get set }
```

## Discussion

This property does not prevent the developer from manually adjusting the magnification value. If magnification exceeds either the maximum or minimum limits for magnification, and allowsMagnification is true, the scroll view temporarily animates the content magnification just past those limits before returning to them. The default value is false.

## See Also

### Zooming the Scroll View

var magnification: CGFloat

The amount by which the content is currently scaled.

func magnify(toFit: NSRect)

Magnifies the content view proportionally such that the given rectangle fits centered in the scroll view.

var maxMagnification: CGFloat

The maximum value to which the content can be magnified.

var minMagnification: CGFloat

The minimum value to which the content can be magnified.

func setMagnification(CGFloat, centeredAt: NSPoint)

Magnify the content by the given amount and center the result on the given point.

