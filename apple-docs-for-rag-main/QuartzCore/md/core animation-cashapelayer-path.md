

- Core Animation
- CAShapeLayer
-  path 

Instance Property

# path

The path defining the shape to be rendered. Animatable.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var path: CGPath? { get set }
```

## Discussion

Unlike most animatable properties, path (as with all CGPath animatable properties) does not support implicit animation.

The path object may be animated using any of the concrete subclasses of CAPropertyAnimation. Paths will interpolate as a linear blend of the “on-line” points; “off-line” points may be interpolated non-linearly (e.g. to preserve continuity of the curve’s derivative). If the two paths have a different number of control points or segments the results are undefined. If the path extends outside the layer bounds it will not automatically be clipped to the layer, only if the normal layer masking rules cause that.

The default value of this property is `nil`.

