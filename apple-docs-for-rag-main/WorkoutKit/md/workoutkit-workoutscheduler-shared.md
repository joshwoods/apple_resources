

- WorkoutKit
- WorkoutScheduler
-  shared 

Type Property

# shared

A shared instance of the workout scheduler.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static let shared: WorkoutScheduler
```

## See Also

### Accessing the scheduler

static var isSupported: Bool

A Boolean value that indicates whether the current device supports scheduled workouts.

func requestAuthorization() async -> WorkoutScheduler.AuthorizationState

Requests authorization to schedule workouts.

var authorizationState: WorkoutScheduler.AuthorizationState

The workout scheduler’s authorization status.

enum AuthorizationState

The workout scheduler’s authorization status.

