

- Accelerate
-  vImage_PerpsectiveTransform 

Structure

# vImage_PerpsectiveTransform

A projective-transformation matrix.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImage_PerpsectiveTransform
```

## Topics

### Creating a projective-transformation structure

init()

Creates a projective-transformation structure.

init(a: Float, b: Float, c: Float, d: Float, tx: Float, ty: Float, vx: Float, vy: Float, v: Float)

Creates a projective-transformation structure from the specified single-precision values.

init?(source: vImage_PerpsectiveTransform.QuadrilateralPoints, destination: vImage_PerpsectiveTransform.QuadrilateralPoints)

Returns a projective-transformation structure that defines the mapping between a source quadrilateral and a destination quadrilateral.

### Inspecting a projective-transformation structure’s properties

var a: Float

The top-left cell in the 3 x 3 transformation matrix.

var b: Float

The top-middle cell in the 3 x 3 transformation matrix.

var c: Float

The middle-left cell in the 3 x 3 transformation matrix.

var d: Float

The middle-middle cell in the 3 x 3 transformation matrix.

var tx: Float

The x-coordinate translation.

var ty: Float

The y-coordinate translation.

var vx: Float

The x-component of the projective vector.

var vy: Float

The y-component of the projective vector.

var v: Float

The homogeneous scale factor.

### Type Aliases

typealias QuadrilateralPoints

A tuple of four points that define a quadrilateral.

### Enumerations

enum Interpolation

Constants that describe the projective-transformation interpolation method.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Sendable

## See Also

### Computing a projective transformation from source and destination quadrilaterals

Transforming an image in three dimensions

Create and use a projective transformation to apply a perspective warp to an image.

func vImageGetPerspectiveWarp(UnsafePointer&lt;(Float, Float)>, UnsafePointer&lt;(Float, Float)>, UnsafeMutablePointer&lt;vImage_PerpsectiveTransform>, vImage_Flags) -> vImage_Error

Returns a projective-transformation structure that defines the mapping between a source quadrilateral and a destination quadrilateral.

