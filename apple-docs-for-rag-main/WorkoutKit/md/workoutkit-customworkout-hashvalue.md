

- WorkoutKit
- CustomWorkout
-  hashValue 

Instance Property

# hashValue

The hashed value of the custom workout.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

## See Also

### Comparing workouts

func hash(into: inout Hasher)

Hashes the essential components of the custom workout by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two custom workouts aren’t equal.

static func == (CustomWorkout, CustomWorkout) -> Bool

Returns a Boolean value that indicates whether two custom workouts are equal.

