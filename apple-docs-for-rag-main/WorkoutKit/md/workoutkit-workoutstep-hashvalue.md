

- WorkoutKit
- WorkoutStep
-  hashValue 

Instance Property

# hashValue

The hashed value of the workout step.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

## See Also

### Comparing workout steps

func hash(into: inout Hasher)

Hashes the essential components of the workout step by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workout steps aren’t equal.

static func == (WorkoutStep, WorkoutStep) -> Bool

Returns a Boolean value that indicates whether two workout steps are equal.

