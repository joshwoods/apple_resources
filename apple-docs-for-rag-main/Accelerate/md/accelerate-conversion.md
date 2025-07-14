

- Accelerate
-  Conversion 

# Conversion

Convert an image to a different format.

## Topics

### Converting any-to-any

Building a basic image conversion workflow

Learn the fundamentals of the convert-any-to-any function by converting a CMYK image to an RGB image.

Converting chroma-subsampled images

Create vImage buffers with the correct dimensions to convert to and from images with subsampled chroma information.

Functions that perform any-to-any conversion

Convert between Core Video or Core Graphics image data of arbitrary color spaces and bit depths.

### Type conversion

Functions that convert between integer planar buffers

Convert the bit depths of planar integer image data.

Functions that convert between integer interleaved buffers

Convert the bit depths of interleaved integer image data.

Functions that convert from integer planar buffers to noninteger planar buffers

Convert planar integer image data to fixed- and floating-point format.

Functions that convert from integer interleaved buffers to noninteger interleaved buffers

Convert interleaved integer image data to fixed- and floating-point format.

Functions that convert between noninteger planar buffers

Convert the bit depths and formats of planar fixed- and floating-point image data.

Functions that convert between noninteger interleaved buffers

Convert the bit depths and formats of interleaved fixed- and floating-point image data.

Functions that convert from noninteger planar buffers to integer planar buffers

Convert planar fixed- and floating-point image data to integer format.

Functions that convert from noninteger interleaved buffers to integer interleaved buffers

Convert interleaved fixed- and floating-point image data to integer format.

### Converting between interleaved and planar formats

Functions that interleave integer planar buffers

Combine discrete integer planar buffers into an interleaved buffer.

Functions that interleave noninteger planar buffers

Combine discrete fixed- and floating-point planar buffers into an interleaved buffer.

Functions that deinterleave integer interleaved buffers

Separate integer interleaved buffers into discrete planar buffers.

Functions that deinterleave noninteger interleaved buffers

Separate fixed- and floating-point interleaved buffers into discrete planar buffers.

### Adding and removing alpha channels

Functions that add an alpha channel to three-channel buffers

Add a constant alpha value or planar alpha buffer to an RGB image.

Functions that remove an alpha channel from four-channel buffers

Remove the alpha channel from an RGBA or ARGB buffer.

### Converting between YCbCr and RGB color spaces

Functions that convert from YCbCr to RGB

Convert image data represented by luma, blue-difference, and red-difference channels to red, green, and blue channels.

Functions that convert from RGB to YCbCr

Convert image data represented by red, green, and blue channels to luma, blue-difference, and red-difference channels.

## See Also

### Conversion Between Image Formats

Building a basic image conversion workflow

Learn the fundamentals of the convert-any-to-any function by converting a CMYK image to an RGB image.

Converting color images to grayscale

Convert an RGB image to grayscale using matrix multiplication.

Applying color transforms to images with a multidimensional lookup table

Precompute translation values to optimize color space conversion and other pointwise operations.

Building a basic image conversion workflow

Learn the fundamentals of the convert-any-to-any function by converting a CMYK image to an RGB image.

Converting luminance and chrominance planes to an ARGB image

Create a displayable ARGB image using the luminance and chrominance information from your device’s camera.

