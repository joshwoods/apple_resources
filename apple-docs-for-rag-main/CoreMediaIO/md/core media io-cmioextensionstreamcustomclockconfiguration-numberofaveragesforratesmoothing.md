

- Core Media I/O
- CMIOExtensionStreamCustomClockConfiguration
-  numberOfAveragesForRateSmoothing 

Instance Property

# numberOfAveragesForRateSmoothing

The number of averages to use for rate smoothing.

Mac Catalyst 15.4+macOS 12.3+

``` source
var numberOfAveragesForRateSmoothing: UInt32 { get }
```

## Discussion

A value of `0` indicates that it uses the default smoothing algorithm.

## See Also

### Inspecting the Configuration

var clockName: String

The name of the clock.

var sourceIdentifier: UUID

A universally unique identifier for the clock.

var getTimeCallMinimumInterval: CMTime

A minimum call time interval for the clock.

var numberOfEventsForRateSmoothing: UInt32

The number of events to use for rate smoothing.

