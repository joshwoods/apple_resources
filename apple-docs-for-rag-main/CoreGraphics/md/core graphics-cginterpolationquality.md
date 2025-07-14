

- Core Graphics
-  CGInterpolationQuality 

Enumeration

# CGInterpolationQuality

Levels of interpolation quality for rendering an image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGInterpolationQuality
```

## Overview

You use the function CGContextSetInterpolationQuality to set the interpolation quality in a graphics context.

## Topics

### Constants

case `default`

The default level of quality.

case none

No interpolation.

case low

A low level of interpolation quality. This setting may speed up image rendering.

case medium

A medium level of interpolation quality. This setting is slower than the low setting but faster than the high setting.

case high

A high level of interpolation quality. This setting may slow down image rendering.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Drawing Images and PDF Content

func draw(CGImage, in: CGRect, byTiling: Bool)

Draws an image in the specified area.

func drawPDFPage(CGPDFPage)

Draws the content of a PDF page into the current graphics context.

var interpolationQuality: CGInterpolationQuality

Returns the current level of interpolation quality for a graphics context.

