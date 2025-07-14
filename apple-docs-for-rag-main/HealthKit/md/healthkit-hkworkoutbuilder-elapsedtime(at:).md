

- HealthKit
- HKWorkoutBuilder
-  elapsedTime(at:) 

Instance Method

# elapsedTime(at:)

Calculates the duration of the workout at the specified time.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func elapsedTime(at date: Date) -> TimeInterval
```

## Parameters 

`date`  

The end date to use to calculate the duration.

## Discussion

The duration of a workout doesn’t include intervals between pause and resume events.

Note

The duration of a workout can decrease when you add past occurrences of pause events.

## See Also

### Starting the workout

func beginCollection(withStart: Date, completion: (Bool, (any Error)?) -> Void)

Sets the workout’s start date and begins building the workout.

var startDate: Date?

The workout’s start date and time.

