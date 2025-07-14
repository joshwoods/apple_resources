

- WorkoutKit
- WorkoutStep
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the workout step by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Comparing workout steps

var hashValue: Int

The hashed value of the workout step.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workout steps aren’t equal.

static func == (WorkoutStep, WorkoutStep) -> Bool

Returns a Boolean value that indicates whether two workout steps are equal.

