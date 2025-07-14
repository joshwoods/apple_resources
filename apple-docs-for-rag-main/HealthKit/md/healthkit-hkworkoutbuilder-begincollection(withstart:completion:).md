

- HealthKit
- HKWorkoutBuilder
-  beginCollection(withStart:completion:) 

Instance Method

# beginCollection(withStart:completion:)

Sets the workout’s start date and begins building the workout.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 5.0+

``` source
func beginCollection(
    withStart startDate: Date,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func beginCollection(at startDate: Date) async throws
```

## See Also

### Starting the workout

var startDate: Date?

The workout’s start date and time.

func elapsedTime(at: Date) -> TimeInterval

Calculates the duration of the workout at the specified time.

