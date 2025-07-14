

- WorkoutKit
- WorkoutGoal
-  hashValue 

Instance Property

# hashValue

The hashed value of the workout goal.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

## See Also

### Comparing workout goals

func hash(into: inout Hasher)

Hashes the essential components of the workout goal by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workout goals aren’t equal.

static func == (WorkoutGoal, WorkoutGoal) -> Bool

Returns a Boolean value that indicates whether two workout goals are equal.

