

- Accelerate
- vImage
- vImage.PixelBuffer
-  equalizeHistogram(binCount:destination:) 

Instance Method

# equalizeHistogram(binCount:destination:)

Equalizes the histogram of a 32-bit planar pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func equalizeHistogram(
    binCount: Int,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.PlanarF`.

## Parameters 

`binCount`  

The number of histogram entries for each channel.

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
    bitsPerComponent: 32,
    bitsPerPixel: 32 * 1,
    colorSpace: CGColorSpaceCreateDeviceGray(),
    bitmapInfo: CGBitmapInfo(rawValue: CGBitmapInfo.byteOrder32Little.rawValue |
                             CGBitmapInfo.floatComponents.rawValue |
                             CGImageAlphaInfo.none.rawValue))!

let buffer = try vImage.PixelBuffer(
    cgImage: srcImage,
    cgImageFormat: &cgImageFormat,
    pixelFormat: vImage.PlanarF.self)

buffer.equalizeHistogram(binCount: 1024,
                         destination: buffer)

let outputImage = buffer.makeCGImage(cgImageFormat: cgImageFormat)
```

## See Also

### Related Documentation

Enhancing image contrast with histogram manipulation

Enhance and adjust the contrast of an image with histogram equalization and contrast stretching.

### Equalization

func equalizeHistogram(destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Equalizes the histogram of an 8-bit planar pixel buffer.

func equalizeHistogram(destination: vImage.PixelBuffer&lt;Format>)

Equalizes the histogram of an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func equalizeHistogram(binCount: Int, destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Equalizes the histogram of a 32-bit-per-channel, 4-channel interleaved pixel buffer.

func equalizeHistogram(destination: vImage.PixelBuffer&lt;Format>)

Equalizes the histogram of a multiple-plane 8-bit pixel buffer.

func equalizeHistogram(binCount: Int, destination: vImage.PixelBuffer&lt;Format>)

Equalizes the histogram of a multiple-plane 32-bit pixel buffer.

