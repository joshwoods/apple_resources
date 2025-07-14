

- Core Haptics
- CHHapticEvent
-  duration 

Instance Property

# duration

The duration of the haptic event.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var duration: TimeInterval { get set }
```

## Discussion

The maximum duration of a continuous haptic event is 30 seconds.

## See Also

### Configuring Haptic Events

var eventParameters: [CHHapticEventParameter]

An array of event parameters, possibly empty.

struct ParameterID

An identifier for an event parameter.

var relativeTime: TimeInterval

The start time of the event, relative to other events in the same pattern.

