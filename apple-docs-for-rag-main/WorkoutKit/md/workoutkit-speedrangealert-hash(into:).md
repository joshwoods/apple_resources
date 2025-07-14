

- WorkoutKit
- SpeedRangeAlert
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the speed range alert by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Comparing alerts

var hashValue: Int

The hashed value of the speed range alert.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two speed range alerts aren’t equal.

static func == (SpeedRangeAlert, SpeedRangeAlert) -> Bool

Returns a Boolean value that indicates whether two speed range alerts are equal.

