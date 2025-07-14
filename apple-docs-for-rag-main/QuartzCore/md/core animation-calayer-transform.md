

- Core Animation
- CALayer
-  transform 

Instance Property

# transform

The transform applied to the layer’s contents. Animatable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var transform: CATransform3D { get set }
```

## Discussion

This property is set to the identity transform by default. Any transformations you apply to the layer occur relative to the layer’s anchor point.

## See Also

### Managing the Layer’s Transform

var sublayerTransform: CATransform3D

Specifies the transform to apply to sublayers when rendering. Animatable.

func affineTransform() -> CGAffineTransform

Returns an affine version of the layer’s transform.

func setAffineTransform(CGAffineTransform)

Sets the layer’s transform to the specified affine transform.

