

- Accelerate
-  vImage_AffineTransform_Double 

Structure

# vImage_AffineTransform_Double

A structure for values that represent a double-precision affine transformation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImage_AffineTransform_Double
```

## Overview

This structure represents the 3x2 matrix :

In 64-bit applications, this structure is just like the Core Graphics CGAffineTransform data structure. In 32-bit applications, the Core Graphics data structure is equivalent to vImage_AffineTransform. Most of the time, you should use the vImage_CGAffineTransform data structure, which changes size depending on architecture.

The CGAffineTransform describes functions for creating and manipulating matrixes of this form.

## Topics

### Initializers

init(a: Double, b: Double, c: Double, d: Double, tx: Double, ty: Double)

Returns a new affine transform.

init()

init(a: CGFloat, b: CGFloat, c: CGFloat, d: CGFloat, tx: CGFloat, ty: CGFloat)

### Affine Transform Matrix Elements

var a: Double

The entry at position `[1,1]` in the matrix.

var b: Double

The entry at position `[1,2]` in the matrix.

var c: Double

The entry at position `[2,1]` in the matrix.

var d: Double

The entry at position `[2,2]` in the matrix.

var tx: Double

The entry at position `[3,1]` in the matrix.

var ty: Double

The entry at position `[3,2]` in the matrix.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct vImage_Buffer

An image buffer that stores an image’s pixel data, dimensions, and row stride.

typealias vImagePixelCount

A type for the number of pixels.

struct vImage_AffineTransform

A structure for values that represent an affine transformation.

typealias vImage_CGAffineTransform

A structure for values that represent a Core Graphics–compatible affine transformation.

typealias vImage_Error

A type for image errors.

typealias vImage_Flags

A type for processing options.

typealias GammaFunction

A type for a gamma function.

typealias ResamplingFilter

A pointer to a resampling filter callback function.

