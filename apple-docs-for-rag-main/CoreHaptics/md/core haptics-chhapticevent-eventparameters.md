

- Core Haptics
- CHHapticEvent
-  eventParameters 

Instance Property

# eventParameters

An array of event parameters, possibly empty.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var eventParameters: [CHHapticEventParameter] { get }
```

## See Also

### Configuring Haptic Events

struct ParameterID

An identifier for an event parameter.

var relativeTime: TimeInterval

The start time of the event, relative to other events in the same pattern.

var duration: TimeInterval

The duration of the haptic event.

