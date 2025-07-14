

- Accelerate
- vImageCVImageFormat
-  vImageCVImageFormat.Format 

Enumeration

# vImageCVImageFormat.Format

Constants that specify the format of a Core Video image format.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum Format
```

## Topics

### RGB format constants

case format16LE555

A little-endian 16-bit, RGB pixel format with 5 bits per channel.

case format16LE565

A little-endian 16-bit, RGB pixel format with 5 bits for red and blue, and 6 bits for green.

case format16BE555

A big-endian 16-bit, RGB pixel format with 5 bits per channel.

case format16BE565

A big-endian 16-bit, RGB pixel format with 5 bits for red and blue, and 6 bits for green.

case format24RGB

A 24-bit, RGB pixel format with 8 bits per channel.

case format24BGR

A 24-bit, BGR pixel format with 8 bits per channel.

case format30RGB

A big-endian 30-bit, RGB pixel format with 10 bits per channel.

case format30RGBLEPackedWideGamut

A little-endian 30-bit, wide-gamut RGB pixel format with 10 bits per channel.

case format48RGB

A big-endian 48-bit, RGB pixel format with 16 bits per channel.

### RGBA and ARGB format constants

case format16LE5551

A little-endian 16-bit, RGBA pixel format with 5 bits per color channel and 1-bit alpha.

case format32ABGR

A 32-bit, ABGR pixel format with 8 bits per channel.

case format32ARGB

A 32-bit, ARGB pixel format with 8 bits per channel.

case format32BGRA

A 32-bit, BGRA pixel format with 8 bits per channel.

case format32RGBA

A 32-bit, RGBA pixel format with 8 bits per channel.

case format64ARGB

A 64-bit, ARGB pixel format with 8 bits per channel.

case format64RGBAHalf

A little-endian 64-bit, RGBA pixel format with 16 bits per channel.

case format128RGBAFloat

A little-endian 128-bit, RGBA pixel format with 32 bits per channel.

case formatARGB2101010LEPacked

A little-endian ARGB2101010 full-range ARGB pixel format.

### Monochrome format constants

case format16Gray

A big-endian 16-bit grayscale pixel format with black equal to zero.

case format32AlphaGray

A big-endian 16-bit grayscale with alpha pixel format with black equal to zero.

### 4:2:0 YpCbCr format constants

case format420YpCbCr8Planar

A planar YpCbCr 4:2:0 pixel format with 8 bits per channel.

case format420YpCbCr8BiPlanarFullRange

A full-range, two-plane YpCbCr 4:2:0 pixel format with 8 bits per channel.

case format420YpCbCr8BiPlanarVideoRange

A video-range, two-plane YpCbCr 4:2:0 pixel format with 8 bits per channel.

case format420YpCbCr8PlanarFullRange

A full-range, planar YpCbCr 4:2:0 pixel format with 8 bits per channel.

case format420YpCbCr10BiPlanarFullRange

A full-range, two-plane YpCbCr 4:2:0 pixel format with 10 bits per channel.

case format420YpCbCr10BiPlanarVideoRange

A video-range, two-plane YpCbCr 4:2:0 pixel format with 10 bits per channel.

### 4:2:2 YpCbCr format constants

case format422YpCbCr8

A component YpCbCr 4:2:2 pixel format with 8 bits per channel and ordered CbYp₀CrYp₁.

case format422YpCbCr8_yuvs

A component YpCbCr 4:2:2 pixel format with 8 bits per channel and ordered Yp₀CbYp₁Cr.

case format422YpCbCr8FullRange

A full-range, component YpCbCr 4:2:2 pixel format with 8 bits per channel.

case format422YpCbCr10

A component YpCbCr 4:2:2 pixel format with 10 bits per channel.

case format422YpCbCr10BiPlanarFullRange

A full-range, two-plane YpCbCr 4:2:2 pixel format with 10 bits per channel.

case format422YpCbCr10BiPlanarVideoRange

A video-range, two-plane YpCbCr 4:2:2 pixel format with 10 bits per channel.

case format422YpCbCr16

A video-range, two-plane YpCbCr 4:2:2 pixel format with 16 bits per channel.

### 4:4:4 YpCbCr format constants

case format444YpCbCr8

A video-range, component YpCbCr 4:4:4 pixel format with 8 bits per channel and ordered CrYpCb.

case format444YpCbCr10

A component YpCbCr 4:4:4 pixel format with 10 bits per channel.

case format444YpCbCr10BiPlanarFullRange

A full-range, two-plane YpCbCr 4:4:4 pixel format with 10 bits per channel.

case format444YpCbCr10BiPlanarVideoRange

A video-range, two-plane YpCbCr 4:4:4 pixel format with 10 bits per channel.

### YpCbCr with alpha format constants

case format422YpCbCr_4A_8BiPlanar

A two-plane pixel format that contains a video-range 8-bit YpCbCr 4:2:2 plane and an 8-bit alpha plane.

case format4444AYpCbCr8

A full-range alpha, video-range luminance and chrominance YpCbCrA 4:4:4:4 pixel format with 8 bits per channel and ordered AYpCbCr.

case format4444YpCbCrA8

A component YpCbCrA 4:4:4:4 pixel format with 8 bits per channel and ordered CbYpCrA.

case format4444YpCbCrA8R

A component YpCbCrA 4:4:4:4 rendering format with 8 bits per channel, full-range alpha, zero-biased YUV, and ordered AYpCbCr.

case format4444AYpCbCr16

A full-range alpha, video-range luminance and chrominance YpCbCrA 4:4:4:4 pixel format with 16 bits per channel and ordered AYpCbCr.

### Bayer format constants

case format14Bayer_BGGR

A little-endian 14-bit Bayer pixel format with even rows ordered blue-green and odd rows ordered green-red.

case format14Bayer_GBRG

A little-endian 14-bit Bayer pixel format with even rows ordered green-blue and odd rows ordered red-green.

case format14Bayer_GRBG

A little-endian 14-bit Bayer pixel format with even rows ordered green-red and odd rows ordered blue-green.

case format14Bayer_RGGB

A little-endian 14-bit Bayer pixel format with even rows ordered red-green and odd rows ordered green-blue.

### Indexed color format constants

case format1Monochrome

A 1-bit indexed pixel format.

case format1IndexedGray_WhiteIsZero

A 1-bit indexed pixel format with white equal to zero.

case format2Indexed

A 2-bit indexed pixel format.

case format2IndexedGray_WhiteIsZero

A 2-bit indexed pixel format with white equal to zero.

case format4Indexed

A 4-bit indexed pixel format.

case format4IndexedGray_WhiteIsZero

A 4-bit indexed pixel format with white equal to zero.

case format8Indexed

An 8-bit indexed pixel format.

case format8IndexedGray_WhiteIsZero

An 8-bit indexed pixel format with white equal to zero.

### Depth format constants

case formatDepthFloat16

A 16-bit depth pixel format that describes the distance to an object in meters.

case formatDepthFloat32

A 32-bit depth pixel format that describes the distance to an object in meters.

### Disparity format constants

case formatDisparityFloat16

A 16-bit disparity pixel format that describes the normalized shift when comparing two images.

case formatDisparityFloat32

A 32-bit disparity pixel format that describes the normalized shift when comparing two images.

### Single-component format constants

case formatOneComponent8

An 8-bit, single-component pixel format with black equal to zero.

case formatOneComponent16Half

A little-endian 16-bit, single-componennt pixel format.

case formatOneComponent32Float

A little-endian 32-bit, single-component pixel format.

### Two-component format constants

case formatTwoComponent8

An 8-bit, two-component pixel format with black equal to zero.

case formatTwoComponent16Half

A little-endian 16-bit, two-component pixel format.

case formatTwoComponent32Float

A little-endian 32-bit, two-component pixel format.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Supporting types

enum ChromaSiting

Constants that specify the chrominance siting of a Core Video image format.

