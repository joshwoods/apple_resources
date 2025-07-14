

- UIKit
- UIView
-  transform 

Instance Property

# transform

Specifies the transform applied to the view, relative to the center of its bounds.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var transform: CGAffineTransform { get set }
```

## Discussion

Use this property to scale or rotate the view’s frame rectangle within its superview’s coordinate system. (To change the position of the view, modify the center property instead.) The default value of this property is `CGAffineTransformIdentity`.

Transformations occur relative to the view’s anchor point. By default, the anchor point is equal to the center point of the frame rectangle. To change the anchor point, modify the anchorPoint property of the view’s underlying CALayer object.

Changes to this property can be animated.

In iOS 8.0 and later, the `transform` property does not affect Auto Layout. Auto layout calculates a view’s alignment rectangle based on its untransformed frame.

Warning

When the value of this property is anything other than the identity transform, the value in the frame property is undefined and should be ignored.

## See Also

### Configuring the bounds and frame rectangles

var frame: CGRect

The frame rectangle, which describes the view’s location and size in its superview’s coordinate system.

var bounds: CGRect

The bounds rectangle, which describes the view’s location and size in its own coordinate system.

var center: CGPoint

The center point of the view’s frame rectangle.

var transform3D: CATransform3D

The three-dimensional transform to apply to the view.

var anchorPoint: CGPoint

The anchor point of the view’s bounds rectangle.

