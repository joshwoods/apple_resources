

- HealthKit
- HKWorkoutBuilder
-  discardWorkout() 

Instance Method

# discardWorkout()

Stops the collection of data and discards the current results without saving the workout.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func discardWorkout()
```

## See Also

### Ending the workout

func endCollection(withEnd: Date, completion: (Bool, (any Error)?) -> Void)

Stops the collection of data, sets the workout’s end date, and deactivates the workout builder.

var endDate: Date?

The workout’s end date and time.

func finishWorkout(completion: (HKWorkout?, (any Error)?) -> Void)

Creates the workout, using the samples and events added to the builder, and saves it to the HealthKit store.

