

- AppKit
- NSScrollView
-  setMagnification(\_:centeredAt:) 

Instance Method

# setMagnification(\_:centeredAt:)

Magnify the content by the given amount and center the result on the given point.

macOS 10.8+

``` source
@MainActor
func setMagnification(
    _ magnification: CGFloat,
    centeredAt point: NSPoint
)
```

## Parameters 

`magnification`  

The amount by which to magnify the content.

`point`  

The point (in content view space) on which to center magnification.

## Discussion

This method scales the content view such that the passed in point (in content view space) remains at the same screen location once the scaling is completed. The resulting magnification value is clipped to the minMagnification and maxMagnification values. To animate the magnification, use the object’s animator.

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

var minMagnification: CGFloat

The minimum value to which the content can be magnified.

