

- Core Haptics
- CHHapticEvent
-  type 

Instance Property

# type

The type of the haptic event.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var type: CHHapticEvent.EventType { get }
```

## Discussion

An audio event can be one of two types: audioCustom or audioContinuous. Haptic events can be hapticTransient or hapticContinuous:

A transient event lasts a split-second and registers as a tap or impulse, whereas a continuous event feels like an extended buzz of longer duration.

## See Also

### Categorizing Haptic Events

struct EventType

The types of audio and haptic event waveforms.

