

- WorkoutKit
- PowerThresholdAlert
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the power threshold alert by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Comparing alerts

var hashValue: Int

The hashed value of the power threshold alert.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two power threshold alerts aren’t equal.

static func == (PowerThresholdAlert, PowerThresholdAlert) -> Bool

Returns a Boolean value that indicates whether two power threshold alerts are equal.

