

- WorkoutKit
- ScheduledWorkoutPlan
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two scheduled plans are equal.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
static func == (a: ScheduledWorkoutPlan, b: ScheduledWorkoutPlan) -> Bool
```

## See Also

### Comparing plans

var hashValue: Int

The hashed value of the scheduled plan.

func hash(into: inout Hasher)

Hashes the essential components of the scheduled plan by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two scheduled plans aren’t equal.

