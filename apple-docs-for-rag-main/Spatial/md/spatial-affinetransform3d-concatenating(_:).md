

- Spatial
- AffineTransform3D
-  concatenating(\_:) 

Instance Method

# concatenating(\_:)

Returns an affine transformation matrix that results from concatenating two existing affine transforms.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func concatenating(_ t2: AffineTransform3D) -> AffineTransform3D
```

## Parameters 

`t2`  

The affine transform that the function concatenates to this affine transform.

## Return Value

The affine transformation matrix that results from concatenating two existing affine transforms.

## Discussion

This function performs the matrix multiplication `self * t2` on the underlying matrices of the two transforms.

## See Also

### Transforming a 3D affine transform structure

struct Axis3D

Constants that describe an axis.

enum AxisWithFactors

Constants that describe the axis of a shear transform.

func changeBasis(from: AffineTransform3D, to: AffineTransform3D) -> AffineTransform3D?

Returns a new affine transform structure by applying a change-of-basis.

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

