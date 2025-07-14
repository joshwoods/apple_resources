

- Spatial
- AffineTransform3D
-  changeBasis(from:to:) 

Instance Method

# changeBasis(from:to:)

Returns a new affine transform structure by applying a change-of-basis.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func changeBasis(
    from: AffineTransform3D = .identity,
    to: AffineTransform3D
) -> AffineTransform3D?
```

## See Also

### Transforming a 3D affine transform structure

struct Axis3D

Constants that describe an axis.

enum AxisWithFactors

Constants that describe the axis of a shear transform.

func concatenating(AffineTransform3D) -> AffineTransform3D

Returns an affine transformation matrix that results from concatenating two existing affine transforms.

func flip(along: Axis3D)

Flips an affine transform along the specified axis.

func flipped(along: Axis3D) -> AffineTransform3D

Returns an affine transform that results from flipping it along the specified axis.

var inverse: AffineTransform3D?

The affine transform’s inverse.

func scaledBy(x: Double, y: Double, z: Double) -> AffineTransform3D

Returns a transform that results from scaling with specified double-precision values.

func sheared(AxisWithFactors) -> AffineTransform3D

Returns an affine transform that results from shearing over an axis by shear factors for the other two axes.

