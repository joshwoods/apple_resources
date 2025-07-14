

- HealthKit
- HKWorkoutBuilder
-  startDate 

Instance Property

# startDate

The workout’s start date and time.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
var startDate: Date? { get }
```

## See Also

### Starting the workout

func beginCollection(withStart: Date, completion: (Bool, (any Error)?) -> Void)

Sets the workout’s start date and begins building the workout.

func elapsedTime(at: Date) -> TimeInterval

Calculates the duration of the workout at the specified time.

