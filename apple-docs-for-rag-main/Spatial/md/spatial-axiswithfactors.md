

- Spatial
-  AxisWithFactors 

Enumeration

# AxisWithFactors

Constants that describe the axis of a shear transform.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
enum AxisWithFactors
```

## Topics

### Enumeration cases

case xAxis(yShearFactor: Double, zShearFactor: Double)

Shears over the x-axis with shear factors for the y- and z-axis.

case yAxis(xShearFactor: Double, zShearFactor: Double)

Shears over the y-axis with shear factors for the x- and z-axis.

case zAxis(xShearFactor: Double, yShearFactor: Double)

Shears over the z-axis with shear factors for the x- and y-axis.

## See Also

### Transforming a 3D affine transform structure

struct Axis3D

Constants that describe an axis.

func changeBasis(from: AffineTransform3D, to: AffineTransform3D) -> AffineTransform3D?

Returns a new affine transform structure by applying a change-of-basis.

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

