

- HealthKit
- HKWorkoutBuilder
-  endDate 

Instance Property

# endDate

The workout’s end date and time.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
var endDate: Date? { get }
```

## See Also

### Ending the workout

func endCollection(withEnd: Date, completion: (Bool, (any Error)?) -> Void)

Stops the collection of data, sets the workout’s end date, and deactivates the workout builder.

func finishWorkout(completion: (HKWorkout?, (any Error)?) -> Void)

Creates the workout, using the samples and events added to the builder, and saves it to the HealthKit store.

func discardWorkout()

Stops the collection of data and discards the current results without saving the workout.

