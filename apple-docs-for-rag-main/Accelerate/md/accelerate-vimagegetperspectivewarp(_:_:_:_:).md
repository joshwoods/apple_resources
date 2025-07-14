

- Accelerate
-  vImageGetPerspectiveWarp(\_:\_:\_:\_:) 

Function

# vImageGetPerspectiveWarp(\_:\_:\_:\_:)

Returns a projective-transformation structure that defines the mapping between a source quadrilateral and a destination quadrilateral.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func vImageGetPerspectiveWarp(
    _ srcPoints: UnsafePointer,
    _ destPoints: UnsafePointer,
    _ transform: UnsafeMutablePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`srcPoints`  

The four source points.

`destPoints`  

The four destination points.

`transform`  

On output, a vImage_PerpsectiveTransform structure that describes the transformation from the source points to the destination points.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Mentioned in 

Transforming an image in three dimensions

## See Also

### Computing a projective transformation from source and destination quadrilaterals

Transforming an image in three dimensions

Create and use a projective transformation to apply a perspective warp to an image.

struct vImage_PerpsectiveTransform

A projective-transformation matrix.

