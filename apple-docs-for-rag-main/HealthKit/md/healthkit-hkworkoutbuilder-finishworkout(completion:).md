

- HealthKit
- HKWorkoutBuilder
-  finishWorkout(completion:) 

Instance Method

# finishWorkout(completion:)

Creates the workout, using the samples and events added to the builder, and saves it to the HealthKit store.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func finishWorkout(completion: @escaping (HKWorkout?, (any Error)?) -> Void)
```

``` source
func finishWorkout() async throws -> HKWorkout?
```

## Mentioned in 

Running workout sessions

Dividing a HealthKit workout into activities

## Discussion

You must call endCollection(withEnd:completion:) before calling this method.

## See Also

### Ending the workout

func endCollection(withEnd: Date, completion: (Bool, (any Error)?) -> Void)

Stops the collection of data, sets the workout’s end date, and deactivates the workout builder.

var endDate: Date?

The workout’s end date and time.

func discardWorkout()

Stops the collection of data and discards the current results without saving the workout.

