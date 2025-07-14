

- WorkoutKit
- PacerWorkout
-  hashValue 

Instance Property

# hashValue

The hashed value of the workout.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

## See Also

### Comparing workouts

func hash(into: inout Hasher)

Hashes the essential components of the workout by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workouts aren’t equal.

static func == (PacerWorkout, PacerWorkout) -> Bool

Returns a Boolean value that indicates whether two workouts are equal.

