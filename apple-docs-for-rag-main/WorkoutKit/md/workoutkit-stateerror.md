

- WorkoutKit
-  StateError 

Enumeration

# StateError

An error that occurs while previewing a workout composition.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
enum StateError
```

## Topics

### Getting the error type

case watchNotPaired

The current device doesn’t have a paired Apple Watch.

case workoutApplicationNotInstalled

The Workout app isn’t installed on this Apple Watch.

### Getting the error description

var localizedDescription: String

A localized description of the error.

### Comparing state errors

var hashValue: Int

The hashed value of the error.

func hash(into: inout Hasher)

Hashes the essential components of the error by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether errors aren’t equal.

static func == (StateError, StateError) -> Bool

Returns a Boolean value that indicates whether errors are equal.

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

