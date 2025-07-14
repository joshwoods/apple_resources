

- WorkoutKit
- HeartRateRangeAlert
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the heart rate range alert by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Comparing heart rate range alerts

var hashValue: Int

The hashed value of the heart rate range alert.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two heart rate range alerts aren’t equal.

static func == (HeartRateRangeAlert, HeartRateRangeAlert) -> Bool

Returns a Boolean value that indicates whether two heart rate range alerts are equal.

