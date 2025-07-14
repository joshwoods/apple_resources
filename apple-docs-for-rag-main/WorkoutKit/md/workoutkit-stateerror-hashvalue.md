

- WorkoutKit
- StateError
-  hashValue 

Instance Property

# hashValue

The hashed value of the error.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

## See Also

### Comparing state errors

func hash(into: inout Hasher)

Hashes the essential components of the error by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether errors aren’t equal.

static func == (StateError, StateError) -> Bool

Returns a Boolean value that indicates whether errors are equal.

