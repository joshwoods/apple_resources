

- HealthKit
- HKWorkoutBuilder
-  endCollection(withEnd:completion:) 

Instance Method

# endCollection(withEnd:completion:)

Stops the collection of data, sets the workout’s end date, and deactivates the workout builder.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func endCollection(
    withEnd endDate: Date,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func endCollection(at endDate: Date) async throws
```

## Mentioned in 

Running workout sessions

## See Also

### Ending the workout

var endDate: Date?

The workout’s end date and time.

func finishWorkout(completion: (HKWorkout?, (any Error)?) -> Void)

Creates the workout, using the samples and events added to the builder, and saves it to the HealthKit store.

func discardWorkout()

Stops the collection of data and discards the current results without saving the workout.

