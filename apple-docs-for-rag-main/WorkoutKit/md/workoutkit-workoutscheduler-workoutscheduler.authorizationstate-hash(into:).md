

- WorkoutKit
- WorkoutScheduler
- WorkoutScheduler.AuthorizationState
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the authorization status by feeding them into the given hash function.

WorkoutKitSwiftiOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## See Also

### Comparing authorization statuses

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two authorization statuses aren’t equal.

var hashValue: Int

The hashed value of the authorization status.

var rawValue: Int

The authorization status’s raw value.

