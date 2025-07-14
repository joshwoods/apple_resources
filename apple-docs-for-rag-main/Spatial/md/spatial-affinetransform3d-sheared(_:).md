

- Spatial
- AffineTransform3D
-  sheared(\_:) 

Instance Method

# sheared(\_:)

Returns an affine transform that results from shearing over an axis by shear factors for the other two axes.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func sheared(_ shear: AxisWithFactors) -> AffineTransform3D
```

## Parameters 

`shear`  

The shear axis and factors.

## Return Value

The affine transform that results from shearing over an axis by shear factors for the other two axes.

## See Also

### Transforming a 3D affine transform structure

struct Axis3D

Constants that describe an axis.

enum AxisWithFactors

Constants that describe the axis of a shear transform.

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

