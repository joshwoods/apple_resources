

- AppKit
-  NSColorRenderingIntent 

Enumeration

# NSColorRenderingIntent

Constants that specify how Cocoa should handle colors that are not located within the destination color space of a graphics context.

macOS 10.5+

``` source
enum NSColorRenderingIntent
```

## Overview

These constants are used by the property colorRenderingIntent.

## Topics

### Constants

case `default`

Use the default rendering intent for the graphics context.

case absoluteColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

case relativeColorimetric

Map colors outside of the gamut of the output device to the closest possible match inside the gamut of the output device.

case perceptual

Preserve the visual relationship between colors by compressing the gamut of the graphics context to fit inside the gamut of the output device.

case saturation

Preserve the relative saturation value of the colors when converting into the gamut of the output device.

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

### Managing Color Rendering

var colorRenderingIntent: NSColorRenderingIntent

The color rendering intent in the graphics context’s graphics state.

