

- Spatial
- AffineTransform3D
-  scaledBy(x:y:z:) 

Instance Method

# scaledBy(x:y:z:)

Returns a transform that results from scaling with specified double-precision values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func scaledBy(
    x: Double = 1,
    y: Double = 1,
    z: Double = 1
) -> AffineTransform3D
```

## Parameters 

`x`  

The double-precision value that specifies the scale along the width dimension.

`y`  

The double-precision value that specifies the scale along the height dimension.

`z`  

The double-precision value that specifies the scale along the depth dimension.

## Return Value

The transform that results from scaling with specified double-precision values.

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

func sheared(AxisWithFactors) -> AffineTransform3D

Returns an affine transform that results from shearing over an axis by shear factors for the other two axes.

