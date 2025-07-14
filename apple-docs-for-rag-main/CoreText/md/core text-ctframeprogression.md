

- Core Text
-  CTFrameProgression 

Enumeration

# CTFrameProgression

Constants that specify frame progression types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTFrameProgression
```

## Overview

The lines of text within a frame may stack for either horizontal or vertical text. Values are enumerated for each stacking type supported by CTFrameProgression. Frames with a progression type that specifies vertical text rotate lines 90 degrees counterclockwise during drawing.

## Topics

### Constants

case topToBottom

Lines stack top to bottom for horizontal text.

case rightToLeft

Lines stack right to left for vertical text.

case leftToRight

Lines stack left to right for vertical text.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

let kCTFrameProgressionAttributeName: CFString

Specifies progression for a frame.

let kCTFramePathFillRuleAttributeName: CFString

The key used to specify the fill rule for a frame.

let kCTFramePathWidthAttributeName: CFString

The key used to specify the frame width.

let kCTFrameClippingPathsAttributeName: CFString

Specifies array of paths to clip frame.

let kCTFramePathClippingPathAttributeName: CFString

Specifies clipping path.

