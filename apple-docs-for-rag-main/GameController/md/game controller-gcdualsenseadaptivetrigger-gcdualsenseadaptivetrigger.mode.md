

- Game Controller
- GCDualSenseAdaptiveTrigger
-  GCDualSenseAdaptiveTrigger.Mode 

Enumeration

# GCDualSenseAdaptiveTrigger.Mode

The possible modes of an adaptive trigger.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+

``` source
enum Mode
```

## Topics

### Modes

case off

Provides no adaptive trigger effects.

case feedback

Provides feedback when the user depresses the trigger equal to, or greater than, the start position.

case weapon

Provides feedback when the user depresses the trigger between the start and the end positions.

case vibration

Vibrates when the user depresses the trigger equal to, or greater than, the start position.

case slopeFeedback

Provides feedback when the user tilts the trigger between the start and the end positions.

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

### Getting the mode

var mode: GCDualSenseAdaptiveTrigger.Mode

The current configuration of the adaptive trigger.

func setModeOff()

Sets the mode to off and stops any trigger effect.

