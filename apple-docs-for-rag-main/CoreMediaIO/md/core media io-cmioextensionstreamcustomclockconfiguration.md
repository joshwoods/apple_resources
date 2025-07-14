

- Core Media I/O
-  CMIOExtensionStreamCustomClockConfiguration 

Class

# CMIOExtensionStreamCustomClockConfiguration

An object that describes the parameters to create a custom clock on the host side.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionStreamCustomClockConfiguration
```

## Topics

### Creating a Clock Configuration

init(clockName: String, sourceIdentifier: UUID, getTimeCallMinimumInterval: CMTime, numberOfEventsForRateSmoothing: UInt32, numberOfAveragesForRateSmoothing: UInt32)

Creates a custom clock configuration.

### Inspecting the Configuration

var clockName: String

The name of the clock.

var sourceIdentifier: UUID

A universally unique identifier for the clock.

var getTimeCallMinimumInterval: CMTime

A minimum call time interval for the clock.

var numberOfEventsForRateSmoothing: UInt32

The number of events to use for rate smoothing.

var numberOfAveragesForRateSmoothing: UInt32

The number of averages to use for rate smoothing.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Inspecting a Stream

var source: (any CMIOExtensionStreamSource)?

The source object for the stream.

var direction: CMIOExtensionStream.Direction

The data-flow direction of the stream.

enum Direction

Constants that define the data-flow direction of the stream.

var clockType: CMIOExtensionStream.ClockType

A clock type for the stream.

enum ClockType

Constants that indicate the clock type of a stream.

var customClockConfiguration: CMIOExtensionStreamCustomClockConfiguration?

An optional custom clock configuration for a stream.

