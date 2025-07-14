

- WorkoutKit
- WorkoutScheduler
-  requestAuthorization() 

Instance Method

# requestAuthorization()

Requests authorization to schedule workouts.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
final func requestAuthorization() async -> WorkoutScheduler.AuthorizationState
```

## See Also

### Accessing the scheduler

static let shared: WorkoutScheduler

A shared instance of the workout scheduler.

static var isSupported: Bool

A Boolean value that indicates whether the current device supports scheduled workouts.

var authorizationState: WorkoutScheduler.AuthorizationState

The workout scheduler’s authorization status.

enum AuthorizationState

The workout scheduler’s authorization status.

