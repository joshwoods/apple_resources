

- Core Media I/O
- CMIOExtensionStreamCustomClockConfiguration
-  init(clockName:sourceIdentifier:getTimeCallMinimumInterval:numberOfEventsForRateSmoothing:numberOfAveragesForRateSmoothing:) 

Initializer

# init(clockName:sourceIdentifier:getTimeCallMinimumInterval:numberOfEventsForRateSmoothing:numberOfAveragesForRateSmoothing:)

Creates a custom clock configuration.

Mac Catalyst 15.4+macOS 12.3+

``` source
init(
    clockName: String,
    sourceIdentifier: UUID,
    getTimeCallMinimumInterval: CMTime,
    numberOfEventsForRateSmoothing: UInt32,
    numberOfAveragesForRateSmoothing: UInt32
)
```

## Parameters 

`clockName`  

The name of the clock.

`sourceIdentifier`  

A universally unique identifier for the clock.

`getTimeCallMinimumInterval`  

A minimum call time interval for the clock. If you query the clock for its current time more often than this interval, it returns an interpolated value.

`numberOfEventsForRateSmoothing`  

The number of events to use for rate smoothing. This value must be greater than `0`.

`numberOfAveragesForRateSmoothing`  

The number of averages to use for rate smoothing. Specify `0`, to use the default smoothing algorithm.

