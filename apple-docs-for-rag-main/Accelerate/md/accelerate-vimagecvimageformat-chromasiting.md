

- Accelerate
- vImageCVImageFormat
-  chromaSiting 

Instance Property

# chromaSiting

The chrominance siting of the Core Video image format.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
var chromaSiting: vImageCVImageFormat.ChromaSiting? { get set }
```

## See Also

### Related Documentation

func vImageCVImageFormat_GetChromaSiting(vImageConstCVImageFormat) -> Unmanaged&lt;CFString>!

Returns the chrominance siting of a Core Video image format.

func vImageCVImageFormat_SetChromaSiting(vImageCVImageFormat, CFString!) -> vImage_Error

Sets the chrominance siting of a Core Video image format.

### Inspecting a Core Video image format’s properties

var channelCount: UInt32

The number of channels, including alpha, for the Core Video image format.

var channels: [vImage.BufferType]

The channels of the Core Video image format.

func channelDescription(bufferType: vImage.BufferType) -> vImageChannelDescription?

Returns the range and clamp limits for a specified channel in a Core Video image format.

var formatCode: UInt32

The four-character code that encodes the pixel format of the Core Video image format.

var colorSpace: CGColorSpace?

The color space of the Core Video image format.

var alphaIsOpaqueHint: Bool

The alpha hint of the Core Video image format.

