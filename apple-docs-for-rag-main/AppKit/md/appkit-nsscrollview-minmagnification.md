

- AppKit
- NSScrollView
-  minMagnification 

Instance Property

# minMagnification

The minimum value to which the content can be magnified.

macOS 10.8+

``` source
@MainActor
var minMagnification: CGFloat { get set }
```

## Discussion

The default value is `0.25`.

## See Also

### Zooming the Scroll View

var allowsMagnification: Bool

Allows the user to magnify the scroll view.

var magnification: CGFloat

The amount by which the content is currently scaled.

func magnify(toFit: NSRect)

Magnifies the content view proportionally such that the given rectangle fits centered in the scroll view.

var maxMagnification: CGFloat

The maximum value to which the content can be magnified.

func setMagnification(CGFloat, centeredAt: NSPoint)

Magnify the content by the given amount and center the result on the given point.

