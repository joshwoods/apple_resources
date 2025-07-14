

- HealthKit
- HKWorkoutBuilder
-  statistics(for:) 

Instance Method

# statistics(for:)

Returns the statistics calculated for matching samples added to the workout.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func statistics(for quantityType: HKQuantityType) -> HKStatistics?
```

## Mentioned in 

Running workout sessions

## See Also

### Associating samples with the workout

func add([HKSample], completion: (Bool, (any Error)?) -> Void)

Adds a sample to be associated with the workout.

func seriesBuilder(for: HKSeriesType) -> HKSeriesBuilder?

Returns the series builder for the specified type, creating a new builder, if necessary.

