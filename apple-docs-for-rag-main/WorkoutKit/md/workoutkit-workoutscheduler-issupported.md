

- WorkoutKit
- WorkoutScheduler
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the current device supports scheduled workouts.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static var isSupported: Bool { get }
```

## See Also

### Accessing the scheduler

static let shared: WorkoutScheduler

A shared instance of the workout scheduler.

func requestAuthorization() async -> WorkoutScheduler.AuthorizationState

Requests authorization to schedule workouts.

var authorizationState: WorkoutScheduler.AuthorizationState

The workout scheduler’s authorization status.

enum AuthorizationState

The workout scheduler’s authorization status.

