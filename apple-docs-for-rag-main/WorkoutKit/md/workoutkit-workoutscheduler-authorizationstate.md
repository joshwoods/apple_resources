

- WorkoutKit
- WorkoutScheduler
-  authorizationState 

Instance Property

# authorizationState

The workout scheduler’s authorization status.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
final var authorizationState: WorkoutScheduler.AuthorizationState { get async }
```

## See Also

### Accessing the scheduler

static let shared: WorkoutScheduler

A shared instance of the workout scheduler.

static var isSupported: Bool

A Boolean value that indicates whether the current device supports scheduled workouts.

func requestAuthorization() async -> WorkoutScheduler.AuthorizationState

Requests authorization to schedule workouts.

enum AuthorizationState

The workout scheduler’s authorization status.

