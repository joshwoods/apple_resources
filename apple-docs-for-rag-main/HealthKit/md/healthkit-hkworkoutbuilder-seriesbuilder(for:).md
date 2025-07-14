

- HealthKit
- HKWorkoutBuilder
-  seriesBuilder(for:) 

Instance Method

# seriesBuilder(for:)

Returns the series builder for the specified type, creating a new builder, if necessary.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func seriesBuilder(for seriesType: HKSeriesType) -> HKSeriesBuilder?
```

## See Also

### Associating samples with the workout

func add([HKSample], completion: (Bool, (any Error)?) -> Void)

Adds a sample to be associated with the workout.

func statistics(for: HKQuantityType) -> HKStatistics?

Returns the statistics calculated for matching samples added to the workout.

