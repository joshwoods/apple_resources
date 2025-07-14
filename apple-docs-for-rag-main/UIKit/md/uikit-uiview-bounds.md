

- UIKit
- UIView
-  bounds 

Instance Property

# bounds

The bounds rectangle, which describes the view’s location and size in its own coordinate system.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var bounds: CGRect { get set }
```

## Mentioned in 

Implementing a Multi-Touch app

## Discussion

The default bounds origin is (0,0) and the size is the same as the size of the rectangle in the frame property. Changing the size portion of this rectangle grows or shrinks the view relative to its center point. Changing the size also changes the size of the rectangle in the frame property to match. The coordinates of the bounds rectangle are always specified in points.

Changing the bounds rectangle automatically redisplays the view without calling its draw(_:) method. If you want UIKit to call the draw(_:) method, set the contentMode property to UIView.ContentMode.redraw.

Changes to this property can be animated.

## See Also

### Configuring the bounds and frame rectangles

var frame: CGRect

The frame rectangle, which describes the view’s location and size in its superview’s coordinate system.

var center: CGPoint

The center point of the view’s frame rectangle.

var transform: CGAffineTransform

Specifies the transform applied to the view, relative to the center of its bounds.

var transform3D: CATransform3D

The three-dimensional transform to apply to the view.

var anchorPoint: CGPoint

The anchor point of the view’s bounds rectangle.

