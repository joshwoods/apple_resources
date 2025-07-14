

- Core Animation
- CALayer
-  affineTransform() 

Instance Method

# affineTransform()

Returns an affine version of the layer’s transform.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func affineTransform() -> CGAffineTransform
```

## Return Value

The affine transform structure that corresponds to the value in the layer’s transform property.

## See Also

### Managing the Layer’s Transform

var transform: CATransform3D

The transform applied to the layer’s contents. Animatable.

var sublayerTransform: CATransform3D

Specifies the transform to apply to sublayers when rendering. Animatable.

func setAffineTransform(CGAffineTransform)

Sets the layer’s transform to the specified affine transform.

