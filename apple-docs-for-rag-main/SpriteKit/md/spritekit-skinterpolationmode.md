

- SpriteKit
-  SKInterpolationMode 

Enumeration

# SKInterpolationMode

The modes used to interpolate between keyframes in the sequence.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum SKInterpolationMode
```

## Topics

### Constants

case linear

Values between two keyframes are interpolated linearly.

case spline

Values between two keyframes using a spline curve.

case step

Values between two keyframes are not interpolated. Instead, the value is that of the most recent keyframe.

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

### Constants

enum SKRepeatMode

The modes used to determine how the sequence repeats.

