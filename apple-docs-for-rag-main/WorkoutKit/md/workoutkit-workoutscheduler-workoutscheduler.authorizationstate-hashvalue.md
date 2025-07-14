

- WorkoutKit
- WorkoutScheduler
- WorkoutScheduler.AuthorizationState
-  hashValue 

Instance Property

# hashValue

The hashed value of the authorization status.

WorkoutKitSwiftiOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## See Also

### Comparing authorization statuses

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two authorization statuses aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of the authorization status by feeding them into the given hash function.

var rawValue: Int

The authorization status’s raw value.

