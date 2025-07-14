

- WorkoutKit
- ScheduledWorkoutPlan
-  hashValue 

Instance Property

# hashValue

The hashed value of the scheduled plan.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

## See Also

### Comparing plans

func hash(into: inout Hasher)

Hashes the essential components of the scheduled plan by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two scheduled plans aren’t equal.

static func == (ScheduledWorkoutPlan, ScheduledWorkoutPlan) -> Bool

Returns a Boolean value that indicates whether two scheduled plans are equal.

