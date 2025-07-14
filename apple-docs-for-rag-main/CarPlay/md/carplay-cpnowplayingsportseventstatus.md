

- CarPlay
-  CPNowPlayingSportsEventStatus 

Class

# CPNowPlayingSportsEventStatus

A representation of the status of a sporting event.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+

``` source
class CPNowPlayingSportsEventStatus
```

## Topics

### Initializers

init(eventStatusText: [String]?, eventStatusImage: UIImage?, eventClock: CPNowPlayingSportsClock?)

Initialize an event status with optional event status text, an optional event status image, and an optional event clock.

### Instance Properties

var eventClock: CPNowPlayingSportsClock?

The event timer, if it applies to this event. See @c CPNowPlayingSportsClock.

var eventStatusImage: UIImage?

An optional event status image for this event, if it applies to this event. For example, a baseball game could display a representation of the bases and outs, indicating how many bases are loaded and the number of outs in the current inning.

var eventStatusText: [String]?

Up to three separate strings for event status may be displayed.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

