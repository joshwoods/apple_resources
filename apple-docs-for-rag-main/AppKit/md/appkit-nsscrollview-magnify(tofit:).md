

- AppKit
- NSScrollView
-  magnify(toFit:) 

Instance Method

# magnify(toFit:)

Magnifies the content view proportionally such that the given rectangle fits centered in the scroll view.

macOS 10.8+

``` source
@MainActor
func magnify(toFit rect: NSRect)
```

## Parameters 

`rect`  

The rectangle (in content view space) to which the content view is magnified.

## Discussion

The resulting magnification value is clipped to the minMagnification and maxMagnification values. To animate the magnification, use the object’s animator.

## See Also

### Zooming the Scroll View

var allowsMagnification: Bool

Allows the user to magnify the scroll view.

var magnification: CGFloat

The amount by which the content is currently scaled.

var maxMagnification: CGFloat

The maximum value to which the content can be magnified.

var minMagnification: CGFloat

The minimum value to which the content can be magnified.

func setMagnification(CGFloat, centeredAt: NSPoint)

Magnify the content by the given amount and center the result on the given point.

