

- WorkoutKit
- WorkoutScheduler
-  WorkoutScheduler.AuthorizationState 

Enumeration

# WorkoutScheduler.AuthorizationState

The workout scheduler’s authorization status.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
enum AuthorizationState
```

## Topics

### Determining the authorization status

case authorized

The user authorized your app to schedule workouts.

case denied

The user denied authorization for scheduling workouts.

case notDetermined

Your app hasn’t yet requested authorization to schedule workouts.

case restricted

The system restricted your app from scheduling workouts.

### Working with the raw value

init?(rawValue: Int)

Creates a new authorization status from the provided value.

typealias RawValue

The data type for the authorization status’s raw value.

### Comparing authorization statuses

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two authorization statuses aren’t equal.

var hashValue: Int

The hashed value of the authorization status.

func hash(into: inout Hasher)

Hashes the essential components of the authorization status by feeding them into the given hash function.

var rawValue: Int

The authorization status’s raw value.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Accessing the scheduler

static let shared: WorkoutScheduler

A shared instance of the workout scheduler.

static var isSupported: Bool

A Boolean value that indicates whether the current device supports scheduled workouts.

func requestAuthorization() async -> WorkoutScheduler.AuthorizationState

Requests authorization to schedule workouts.

var authorizationState: WorkoutScheduler.AuthorizationState

The workout scheduler’s authorization status.

