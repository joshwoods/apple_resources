

- WorkoutKit
- WorkoutScheduler
- WorkoutScheduler.AuthorizationState
-  rawValue 

Instance Property

# rawValue

The authorization status’s raw value.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var rawValue: Int { get }
```

## See Also

### Comparing authorization statuses

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two authorization statuses aren’t equal.

var hashValue: Int

The hashed value of the authorization status.

func hash(into: inout Hasher)

Hashes the essential components of the authorization status by feeding them into the given hash function.

