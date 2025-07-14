

- Accelerate
- vImageCVImageFormat
-  channelDescription(bufferType:) 

Instance Method

# channelDescription(bufferType:)

Returns the range and clamp limits for a specified channel in a Core Video image format.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func channelDescription(bufferType: vImage.BufferType) -> vImageChannelDescription?
```

## Parameters 

`bufferType`  

The source buffer type.

## Return Value

A vImageChannelDescription structure that describes the range and clamp limits for the specified channel.

## Discussion

Use this function to return the vImageChannelDescription description for a specified channel in a Core Video format.

For example, the following code prints the description of each channel in a kCVPixelFormatType_420YpCbCr8Planar Core Video image format:

```
let cvImageFormat = vImageCVImageFormat.make(
    format: .format420YpCbCr8Planar,
    matrix: kvImage_ARGBToYpCbCrMatrix_ITU_R_709_2.pointee,
    chromaSiting: .center,
    colorSpace: CGColorSpace(name: CGColorSpace.sRGB)!,
    alphaIsOpaqueHint: true)!

// Prints:
//    luminance   vImageChannelDescription(min: 0.0, zero: 16.0, full: 235.0, max: 255.0)
//    Cb          vImageChannelDescription(min: 0.0, zero: 128.0, full: 240.0, max: 255.0)
//    Cr          vImageChannelDescription(min: 0.0, zero: 128.0, full: 240.0, max: 255.0)
for channel in cvImageFormat.channels {
    let desc = cvImageFormat.channelDescription(bufferType: channel)!
    print("\(channel) \t\t \(desc)")
}
```

## See Also

### Related Documentation

func vImageCVImageFormat_CopyChannelDescription(vImageCVImageFormat, UnsafePointer&lt;vImageChannelDescription>, vImageBufferTypeCode) -> vImage_Error

Copies the channel description for a particular channel type to an image format.

### Inspecting a Core Video image format’s properties

var channelCount: UInt32

The number of channels, including alpha, for the Core Video image format.

var channels: [vImage.BufferType]

The channels of the Core Video image format.

var formatCode: UInt32

The four-character code that encodes the pixel format of the Core Video image format.

var chromaSiting: vImageCVImageFormat.ChromaSiting?

The chrominance siting of the Core Video image format.

var colorSpace: CGColorSpace?

The color space of the Core Video image format.

var alphaIsOpaqueHint: Bool

The alpha hint of the Core Video image format.

