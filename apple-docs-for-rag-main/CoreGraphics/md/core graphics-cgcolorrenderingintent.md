

- Core Graphics
-  CGColorRenderingIntent 

Enumeration

# CGColorRenderingIntent

Handling options for colors that are not located within the destination color space of a graphics context.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGColorRenderingIntent
```

## Overview

The rendering intent specifies how Quartz should handle colors that are not located within the gamut of the destination color space of a graphics context. It determines the exact method used to map colors from one color space to another. If you do not explicitly set the rendering intent by calling the function setRenderingIntent(_:), the graphics context uses the relative colorimetric rendering intent, except when drawing sampled images.

## Topics

### Constants

case defaultIntent

The default rendering intent for the graphics context.

case absoluteColorimetric

case relativeColorimetric

case perceptual

Preserve the visual relationship between colors by compressing the gamut of the graphics context to fit inside the gamut of the output device. Perceptual intent is good for photographs and other complex, detailed images.

case saturation

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

