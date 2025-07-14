

- WorkoutKit
- ScheduledWorkoutPlan
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the scheduled plan by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Comparing plans

var hashValue: Int

The hashed value of the scheduled plan.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two scheduled plans aren’t equal.

static func == (ScheduledWorkoutPlan, ScheduledWorkoutPlan) -> Bool

Returns a Boolean value that indicates whether two scheduled plans are equal.

