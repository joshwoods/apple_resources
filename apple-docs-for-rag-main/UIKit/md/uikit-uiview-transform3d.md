

- UIKit
- UIView
-  transform3D 

Instance Property

# transform3D

The three-dimensional transform to apply to the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var transform3D: CATransform3D { get set }
```

## Discussion

The default value of this property is CATransform3DIdentity.

## See Also

### Configuring the bounds and frame rectangles

var frame: CGRect

The frame rectangle, which describes the view’s location and size in its superview’s coordinate system.

var bounds: CGRect

The bounds rectangle, which describes the view’s location and size in its own coordinate system.

var center: CGPoint

The center point of the view’s frame rectangle.

var transform: CGAffineTransform

Specifies the transform applied to the view, relative to the center of its bounds.

var anchorPoint: CGPoint

The anchor point of the view’s bounds rectangle.

