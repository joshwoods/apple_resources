

- WorkoutKit
- SwimBikeRunWorkout
- SwimBikeRunWorkout.Activity
-  hashValue 

Instance Property

# hashValue

The hashed value of the activity.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

## See Also

### Comparing activities

func hash(into: inout Hasher)

Hashes the essential components of the activity by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two activities aren’t equal.

static func == (SwimBikeRunWorkout.Activity, SwimBikeRunWorkout.Activity) -> Bool

Returns a Boolean value that indicates whether two activities are equal.

