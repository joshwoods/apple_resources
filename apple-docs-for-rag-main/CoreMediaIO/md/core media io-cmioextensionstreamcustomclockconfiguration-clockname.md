

- Core Media I/O
- CMIOExtensionStreamCustomClockConfiguration
-  clockName 

Instance Property

# clockName

The name of the clock.

Mac Catalyst 15.4+macOS 12.3+

``` source
var clockName: String { get }
```

## See Also

### Inspecting the Configuration

var sourceIdentifier: UUID

A universally unique identifier for the clock.

var getTimeCallMinimumInterval: CMTime

A minimum call time interval for the clock.

var numberOfEventsForRateSmoothing: UInt32

The number of events to use for rate smoothing.

var numberOfAveragesForRateSmoothing: UInt32

The number of averages to use for rate smoothing.

