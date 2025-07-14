

- Core Text
-  CTFramePathFillRule 

Enumeration

# CTFramePathFillRule

These constants specify the fill rule used by a frame

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTFramePathFillRule
```

## Overview

When a path intersects with itself, the client should specify which rule to use for deciding the area of the path.

## Topics

### Enumeration Cases

case evenOdd

Paints the area using the even-odd fill rule.

case windingNumber

Paints the area using the nonzero winding number rule.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

