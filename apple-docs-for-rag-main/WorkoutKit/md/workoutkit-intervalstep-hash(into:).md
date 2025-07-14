

- WorkoutKit
- IntervalStep
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the interval step by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Comparing interval steps

var hashValue: Int

The hashed value of the interval step.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two interval steps aren’t equal.

static func == (IntervalStep, IntervalStep) -> Bool

Returns a Boolean value that indicates whether two interval steps are equal.

