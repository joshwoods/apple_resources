

- Core Animation
- CALayer
-  sublayerTransform 

Instance Property

# sublayerTransform

Specifies the transform to apply to sublayers when rendering. Animatable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var sublayerTransform: CATransform3D { get set }
```

## Discussion

You typically use this property to add perspective and other viewing effects to embedded layers. You add perspective by setting the sublayer transform to the desired projection matrix. The default value of this property is the identity transform.

## See Also

### Managing the Layer’s Transform

var transform: CATransform3D

The transform applied to the layer’s contents. Animatable.

func affineTransform() -> CGAffineTransform

Returns an affine version of the layer’s transform.

func setAffineTransform(CGAffineTransform)

Sets the layer’s transform to the specified affine transform.

