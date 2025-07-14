

- Core Media I/O
- CMIOExtensionStreamCustomClockConfiguration
-  getTimeCallMinimumInterval 

Instance Property

# getTimeCallMinimumInterval

A minimum call time interval for the clock.

Mac Catalyst 15.4+macOS 12.3+

``` source
var getTimeCallMinimumInterval: CMTime { get }
```

## Discussion

If you query the clock for its current time more often than this interval, the system returns an interpolated value.

## See Also

### Inspecting the Configuration

var clockName: String

The name of the clock.

var sourceIdentifier: UUID

A universally unique identifier for the clock.

var numberOfEventsForRateSmoothing: UInt32

The number of events to use for rate smoothing.

var numberOfAveragesForRateSmoothing: UInt32

The number of averages to use for rate smoothing.

