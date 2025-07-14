

- Core Media I/O
- CMIOExtensionStreamCustomClockConfiguration
-  numberOfEventsForRateSmoothing 

Instance Property

# numberOfEventsForRateSmoothing

The number of events to use for rate smoothing.

Mac Catalyst 15.4+macOS 12.3+

``` source
var numberOfEventsForRateSmoothing: UInt32 { get }
```

## Discussion

The property value is always greater than `0`.

## See Also

### Inspecting the Configuration

var clockName: String

The name of the clock.

var sourceIdentifier: UUID

A universally unique identifier for the clock.

var getTimeCallMinimumInterval: CMTime

A minimum call time interval for the clock.

var numberOfAveragesForRateSmoothing: UInt32

The number of averages to use for rate smoothing.

