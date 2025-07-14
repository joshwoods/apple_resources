

- Core Haptics
- CHHapticEvent
-  relativeTime 

Instance Property

# relativeTime

The start time of the event, relative to other events in the same pattern.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var relativeTime: TimeInterval { get set }
```

## Discussion

A relativeTime of zero indicates immediate playback. Another haptic event starting one second later would have a relativeTime of `1`.

## See Also

### Configuring Haptic Events

var eventParameters: [CHHapticEventParameter]

An array of event parameters, possibly empty.

struct ParameterID

An identifier for an event parameter.

var duration: TimeInterval

The duration of the haptic event.

