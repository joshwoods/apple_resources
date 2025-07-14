

- Core Media I/O
- CMIOExtensionStreamCustomClockConfiguration
-  sourceIdentifier 

Instance Property

# sourceIdentifier

A universally unique identifier for the clock.

Mac Catalyst 15.4+macOS 12.3+

``` source
var sourceIdentifier: UUID { get }
```

## See Also

### Inspecting the Configuration

var clockName: String

The name of the clock.

var getTimeCallMinimumInterval: CMTime

A minimum call time interval for the clock.

var numberOfEventsForRateSmoothing: UInt32

The number of events to use for rate smoothing.

var numberOfAveragesForRateSmoothing: UInt32

The number of averages to use for rate smoothing.

