

- AVFoundation
-  AVCaptureColorSpace 

Enumeration

# AVCaptureColorSpace

An enumeration of color spaces a device can support.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
enum AVCaptureColorSpace
```

## Overview

By default, a capture session automatically enables wide-gamut capture for supported devices and capture workflows.

## Topics

### Color Spaces

case sRGB

The standard RGB color space.

case P3_D65

The P3 D65 wide color space that uses Illuminant D65 as the white point.

case HLG_BT2020

The BT.2020 wide color space that uses Illuminant D65 as the white point and Hybrid Log-Gamma (HLG) as the transfer function.

case appleLog

The Apple Log Color space, which uses BT2020 as the color primaries, and an Apple-defined Log curve as a transfer function.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Color Space Settings

var activeColorSpace: AVCaptureColorSpace

The currently active color space for capture.

