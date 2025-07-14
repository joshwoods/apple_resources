

- Accelerate
- vImage
- vImage.PixelBuffer
-  equalizeHistogram(destination:) 

Instance Method

# equalizeHistogram(destination:)

Equalizes the histogram of a multiple-plane 8-bit pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func equalizeHistogram(destination: vImage.PixelBuffer)
```

Available when `Format` conforms to `MultiplePlanePixelFormat` and `Format.ComponentType` is `UInt8`.

## Parameters 

`destination`  

The destination pixel buffer.

## Discussion

Use this function to transform an image so that its histogram is more uniformly distributed across the entire range of values.

For example, the following code equalizes the histogram of an image:

```
let srcImage =  imageLiteral(resourceName: " ... ").cgImage(
    forProposedRect: nil,
    context: nil,
    hints: nil)!

var cgImageFormat = vImage_CGImageFormat(
    bitsPerComponent: 8,
    bitsPerPixel: 8 * 3,
    colorSpace: CGColorSpaceCreateDeviceRGB(),
    bitmapInfo: CGBitmapInfo(rawValue: CGImageAlphaInfo.none.rawValue))!

let interleavedBuffer = try vImage.PixelBuffer(
    cgImage: srcImage,
    cgImageFormat: &cgImageFormat,
    pixelFormat: vImage.Interleaved8x3.self)

let multiplaneBuffer = vImage.PixelBuffer(
    interleavedBuffer: interleavedBuffer)

multiplaneBuffer.equalizeHistogram(destination: multiplaneBuffer)

multiplaneBuffer.convert(to: interleavedBuffer)

```

## See Also

### Related Documentation

Enhancing image contrast with histogram manipulation

Enhance and adjust the contrast of an image with histogram equalization and contrast stretching.

### Equalization

func equalizeHistogram(destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Equalizes the histogram of an 8-bit planar pixel buffer.

func equalizeHistogram(binCount: Int, destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Equalizes the histogram of a 32-bit planar pixel buffer.

func equalizeHistogram(destination: vImage.PixelBuffer&lt;Format>)

Equalizes the histogram of an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func equalizeHistogram(binCount: Int, destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Equalizes the histogram of a 32-bit-per-channel, 4-channel interleaved pixel buffer.

func equalizeHistogram(binCount: Int, destination: vImage.PixelBuffer&lt;Format>)

Equalizes the histogram of a multiple-plane 32-bit pixel buffer.

