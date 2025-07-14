

- Accelerate
- Conversion
-  Converting chroma-subsampled images 

Article

# Converting chroma-subsampled images

Create vImage buffers with the correct dimensions to convert to and from images with subsampled chroma information.

## Overview

When you work with video data, you often work with images represented by separate luminance (Y) and chrominance (CbCr) information at different resolutions. The vImage library provides functionality to convert images in this format to an interleaved RGB format, which simplifies applying some image-processing operations.

Alternatively, other image transformations, such as adjusting saturation, require that you convert an RGB image to YCbCr. Reducing the resolution of the chrominance information can also improve the performance of your app because you’re only processing half or a quarter of the number of pixels.

*Chroma subsampling* describes the encoding that compresses image data by reducing the resolution of the chrominance information. Chroma subsampling relies on the fact that human vision is less sensitive to color than luminance.

The code in this article uses the 4:2:0 subsampling scheme, which means there’s one Cb and one Cr pixel for every four luminance pixels. That is, each chrominance channel is half of the width and half of the height of the luminance channel. For example, 4:2:0 subsampling represents a 4 x 2 image with a 4 x 2 luminance channel and two 2 x 1 chrominance channels:

The images below show the 4:2:0 subsampling scheme applied to a photograph. The *Y* luminance channel has the same resolution as the original image. However, the *Cb* and *Cr* chrominance channels have a lower resolution. For each 2 x 2 square of pixels in the luminance channel, the chrominance channels only contain a single pixel. Therefore, the chrominance channels are a quarter of the size of the luminance channel.

### Define the Core Video and Core Graphics image formats

If you’re working with CVPixelBuffer objects, the vImage library provides the vImageCVImageFormat_CreateWithCVPixelBuffer(_:) and make(buffer:) functions that generate a vImageCVImageFormat structure from a Core Video pixel buffer. However, the code in this article defines a vImageCVImageFormat.Format.format420YpCbCr8PlanarFullRange Core Video image format that describes the YpCbCr image. The code below also defines an 8-bit-per-channel RGB Core Graphics image format:

```
var cgImageFormat = vImage_CGImageFormat(
    bitsPerComponent: 8,
    bitsPerPixel: 8 * 3,
    colorSpace: CGColorSpaceCreateDeviceRGB(),
    bitmapInfo: CGBitmapInfo(rawValue: CGImageAlphaInfo.none.rawValue))!

let cvImageFormat = vImageCVImageFormat.make(
    format: .format420YpCbCr8PlanarFullRange,
    matrix: kvImage_ARGBToYpCbCrMatrix_ITU_R_601_4.pointee,
    chromaSiting: .center,
    colorSpace: CGColorSpaceCreateDeviceRGB(),
    alphaIsOpaqueHint: true)!
```

### Perform the Core Graphics to Core Video conversion

Use the Core Video and Core Graphics image format descriptions to create an any-to-any vImageConverter instance that converts from Core Graphics to Core Video image format.

```
let cgToCvConverter = try vImageConverter.make(sourceFormat: cgImageFormat,
                                               destinationFormat: cvImageFormat)
```

The converter provides the destinationBufferCount property that you use to generate the correct number of destination buffers. Although the chrominance size is a quarter of the luminance sizes, declare the sizes of all three pixel buffers as the source image size.

```
let ypCbCr8PlanarBuffers = (0 ..(size: rgbSourceBuffer.size)
}
```

Important

The source and destination vlmage buffers that you pass to an any-to-any conversion must all share the same dimensions.

In the code below, `rgbSourceBuffer` is a vImage.PixelBuffer with a format of vImage.Interleaved8x3 (that matches the vImage_CGImageFormat structure above) which contains a source image. Call the convert(from:to:) method to populate the destination buffers.

```
try cgToCvConverter.convert(from: [rgbSourceBuffer],
                            to: ypCbCr8PlanarBuffers)
```

On return, the three pixel buffers in the `ypCbCr8PlanarBuffers` array contain the luminance and two chrominance channels. The image below shows the luminance channel (left), the Cb channel (middle), and the Cr channel (right):

### Apply an operation to the subsampled chrominance channels

Although the two chrominance channels are the same size as the full-sized luminance channel, they only contain a quarter of the data. If you’re applying an image-processing operation to the Cb and Cr channels, use the withUnsafeRegionOfInterest(_:_:) method. This ensures that you’re not processing unused pixels. The code below reduces the saturation of the image using the technique discussed in Adjusting saturation and applying tone mapping:

```
let saturation = Float(0.25)
let preBias = -128
let divisor = 0x1000
let postBias = 128 * divisor
let factor = Int(saturation * Float(divisor))

// Define a region of interest that's a quarter of the area of the
// luminance channel.
let roi = CGRect(x: 0, y: 0,
                 width: ypCbCr8PlanarBuffers[0].width / 2,
                 height: ypCbCr8PlanarBuffers[0].height / 2)

// Indices 1 and 2 refer to the Cb and Cr buffers, respectively.
for index in [1, 2] {
    ypCbCr8PlanarBuffers[index].withUnsafeRegionOfInterest(roi) { buffer in
        buffer.multiply(by: factor,
                        divisor: divisor,
                        preBias: preBias,
                        postBias: postBias,
                        destination: buffer)
    }
}
```

For more information about limiting the effect of vImage operations to rectangular regions of interest, see Applying vImage operations to regions of interest.

### Perform the Core Video to Core Graphics conversion

To convert the YpCbCr buffers to an RGB buffer, create a converter with the Core Video image format as the source and the Core Graphics image format as the destination. Call the convert(from:to:) method as above, but specify the `ypCbCr8PlanarBuffers` array as the source and an 8-bit-per-channel interleaved buffer as the destination.

```
let cvToCgConverter = try vImageConverter.make(sourceFormat: cvImageFormat,
                                               destinationFormat: cgImageFormat)

let rgbDestinationBuffer = vImage.PixelBuffer(
    size: ypCbCr8PlanarBuffers.first!.size)

try cvToCgConverter.convert(from: ypCbCr8PlanarBuffers,
                            to: [rgbDestinationBuffer])
```

On return, `rgbDestinationBuffer` contains the desaturated version (right) of the original image (left).

## See Also

### Converting any-to-any

Building a basic image conversion workflow

Learn the fundamentals of the convert-any-to-any function by converting a CMYK image to an RGB image.

Functions that perform any-to-any conversion

Convert between Core Video or Core Graphics image data of arbitrary color spaces and bit depths.

