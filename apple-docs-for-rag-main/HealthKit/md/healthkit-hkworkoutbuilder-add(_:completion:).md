

- HealthKit
- HKWorkoutBuilder
-  add(\_:completion:) 

Instance Method

# add(\_:completion:)

Adds a sample to be associated with the workout.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func add(
    _ samples: [HKSample],
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func addSamples(_ samples: [HKSample]) async throws
```

## Mentioned in 

Running workout sessions

## See Also

### Associating samples with the workout

func seriesBuilder(for: HKSeriesType) -> HKSeriesBuilder?

Returns the series builder for the specified type, creating a new builder, if necessary.

func statistics(for: HKQuantityType) -> HKStatistics?

Returns the statistics calculated for matching samples added to the workout.

