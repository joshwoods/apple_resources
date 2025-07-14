

- SpriteKit
-  SKRepeatMode 

Enumeration

# SKRepeatMode

The modes used to determine how the sequence repeats.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum SKRepeatMode
```

## Topics

### Constants

case clamp

When a sample is calculated, the time value is clamped to the range of time values found in the sequence. For example, if the last keyframe’s time value is `0.5`, a sample at any time value from `0.5` to `1.0` returns the last keyframe’s value.

case loop

When a sample is calculated, the sequence loops back to the beginning of the sequence. For example, if the last keyframe’s time value is `0.5`, then a sample at any time value from `0.5` to `1.0` returns the same value as the sequence did from `0.0` to `0.5`.

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

enum SKInterpolationMode

The modes used to interpolate between keyframes in the sequence.

