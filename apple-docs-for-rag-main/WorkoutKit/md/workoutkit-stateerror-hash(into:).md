

- WorkoutKit
- StateError
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the error by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Comparing state errors

var hashValue: Int

The hashed value of the error.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether errors aren’t equal.

static func == (StateError, StateError) -> Bool

Returns a Boolean value that indicates whether errors are equal.

