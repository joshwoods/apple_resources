

- UIKit
- UIView
-  center 

Instance Property

# center

The center point of the view’s frame rectangle.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var center: CGPoint { get set }
```

## Discussion

The center point is specified in points in the coordinate system of its superview. Setting this property updates the origin of the rectangle in the frame property appropriately.

Use this property, instead of the frame property, when you want to change the position of a view. The center point is always valid, even when scaling or rotation factors are applied to the view’s transform. Changes to this property can be animated.

## See Also

### Configuring the bounds and frame rectangles

var frame: CGRect

The frame rectangle, which describes the view’s location and size in its superview’s coordinate system.

var bounds: CGRect

The bounds rectangle, which describes the view’s location and size in its own coordinate system.

var transform: CGAffineTransform

Specifies the transform applied to the view, relative to the center of its bounds.

var transform3D: CATransform3D

The three-dimensional transform to apply to the view.

var anchorPoint: CGPoint

The anchor point of the view’s bounds rectangle.

