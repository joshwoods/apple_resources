

- WorkoutKit
- SwimBikeRunWorkout
- SwimBikeRunWorkout.Activity
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the activity by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Comparing activities

var hashValue: Int

The hashed value of the activity.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two activities aren’t equal.

static func == (SwimBikeRunWorkout.Activity, SwimBikeRunWorkout.Activity) -> Bool

Returns a Boolean value that indicates whether two activities are equal.

