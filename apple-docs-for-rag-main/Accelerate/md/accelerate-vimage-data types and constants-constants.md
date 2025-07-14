

- Accelerate
- vImage
-  Data Types and Constants 

API Collection

# Data Types and Constants

Look up type aliases, data types, and constants the vImage library uses.

## Overview

The vImage library defines data types for planar and interleaved pixel types, a resampling callback filter, and an affine transform. vImage provides constants that specify errors and flags that you pass to a function to specify a variety of processing options.

## Topics

### Pixel Formats

typealias Pixel_8

A type for a planar, 8-bits-per-channel, unsigned pixel.

typealias Pixel_88

A type for a two-channel, 8-bits-per-channel, unsigned pixel.

typealias Pixel_8888

A type for a four-channel, 8-bits-per-channel, unsigned pixel.

typealias Pixel_F

A type for a planar, 32-bits-per-channel, floating-point pixel.

typealias Pixel_FFFF

A type for a four-channel, 32-bits-per-channel, floating-point pixel.

typealias Pixel_32U

A type you use for the XRGB2101010 format.

typealias Pixel_16U

A type for a planar, 16-bits-per-channel, unsigned pixel.

typealias Pixel_ARGB_16U

A type for a four-channel, 16-bits-per-channel, unsigned pixel.

typealias Pixel_16U16U

A type for a two-channel, 16-bits-per-channel, unsigned pixel.

typealias Pixel_16Q12

A type for a signed 16-bit, fixed-point number with 12 bits of fractional precision.

typealias Pixel_16S

A type for a planar, 16-bits-per-channel, signed pixel.

typealias Pixel_ARGB_16S

A type for a four-channel, 16-bits-per-channel, signed pixel.

typealias Pixel_16F

typealias Pixel_16F16F

typealias Pixel_16S16S

typealias Pixel_ARGB_16F

typealias Pixel_FF

### Data Types

struct vImage_Buffer

An image buffer that stores an image’s pixel data, dimensions, and row stride.

typealias vImagePixelCount

A type for the number of pixels.

struct vImage_AffineTransform

A structure for values that represent an affine transformation.

struct vImage_AffineTransform_Double

A structure for values that represent a double-precision affine transformation.

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

### Constants

Error codes

Error codes that vImage functions return when an operation fails.

Core Video Image Format Errors

Processing Flags

Set flags on vImage operations to specify processing options.

Dithering Methods

Specify the dithering method some vImage conversion functions use.

Availability Flags

Obtain the availability of particular vImage features.

Decode Arrays

Specify the decode array constant to use with 16Q12-formatted data.

Buffer Types

Look up buffer type codes vImage conversions provide.

typealias vImageMatrixType

An enumeration of RGB -\> Y’CbCr conversion matrix types.

typealias vImage_WarpInterpolation

Constants for selecting the interpolation mode

## See Also

### Related Documentation

vImage Programming Guide

