

- Accelerate
-  vImageChannelDescription 

Structure

# vImageChannelDescription

A description of the range and clamp limits for a pixel format.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImageChannelDescription
```

## Overview

A vImageChannelDescription structure describes the range and clamp limits for each channel in a Core Video image format. The min and max properties define the clamping limits, and functions clamp values to min…max. The zero and full values specify the normal range and bias for a format, and encode `0.0` and `1.0`, respectively (`0.0` and `0.5` for chrominance).

## Topics

### Creating a channel description

init(min: CGFloat, zero: CGFloat, full: CGFloat, max: CGFloat)

Returns a structure that describes the range and clamp limits for a pixel format.

init()

Returns an empty structure that describes the range and clamp limits for a pixel format.

### Instance properties

var min: CGFloat

The minimum encoded value.

var zero: CGFloat

The encoding for the value zero.

var full: CGFloat

The encoding for the value one.

var max: CGFloat

The maximum encoded value.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Querying and setting channel information

func vImageCVImageFormat_GetChannelCount(vImageConstCVImageFormat) -> UInt32

Returns the number of channels, including alpha, for the Core Video image format.

func vImageCVImageFormat_GetChannelDescription(vImageConstCVImageFormat, vImageBufferTypeCode) -> UnsafePointer&lt;vImageChannelDescription>!

Returns the channel description for a particular channel type.

func vImageCVImageFormat_CopyChannelDescription(vImageCVImageFormat, UnsafePointer&lt;vImageChannelDescription>, vImageBufferTypeCode) -> vImage_Error

Copies the channel description for a particular channel type to an image format.

func vImageCVImageFormat_GetChannelNames(vImageConstCVImageFormat) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns the names of the channels of a Core Video image format.

