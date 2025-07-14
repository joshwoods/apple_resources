

- Accelerate
- vImageCVImageFormat
-  channels 

Instance Property

# channels

The channels of the Core Video image format.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
var channels: [vImage.BufferType] { get }
```

## Discussion

For example, the following code prints the channels in a kCVPixelFormatType_420YpCbCr8Planar Core Video image format:

```
let cvImageFormat = vImageCVImageFormat.make(
    format: .format420YpCbCr8Planar,
    matrix: kvImage_ARGBToYpCbCrMatrix_ITU_R_709_2.pointee,
    chromaSiting: .center,
    colorSpace: CGColorSpace(name: CGColorSpace.sRGB)!,
    alphaIsOpaqueHint: true)!

// Prints "channels [Accelerate.vImage.BufferType.luminance,
//                   Accelerate.vImage.BufferType.Cb,
//                   Accelerate.vImage.BufferType.Cr]".
print("channels \(cvImageFormat.channels)")
```

## See Also

### Related Documentation

func vImageCVImageFormat_GetChannelNames(vImageConstCVImageFormat) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns the names of the channels of a Core Video image format.

### Inspecting a Core Video image format’s properties

var channelCount: UInt32

The number of channels, including alpha, for the Core Video image format.

func channelDescription(bufferType: vImage.BufferType) -> vImageChannelDescription?

Returns the range and clamp limits for a specified channel in a Core Video image format.

var formatCode: UInt32

The four-character code that encodes the pixel format of the Core Video image format.

var chromaSiting: vImageCVImageFormat.ChromaSiting?

The chrominance siting of the Core Video image format.

var colorSpace: CGColorSpace?

The color space of the Core Video image format.

var alphaIsOpaqueHint: Bool

The alpha hint of the Core Video image format.

