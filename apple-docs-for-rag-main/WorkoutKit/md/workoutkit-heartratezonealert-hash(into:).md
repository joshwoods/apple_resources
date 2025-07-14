

- WorkoutKit
- HeartRateZoneAlert
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the heart rate zone alert by feeding them into the given hash function.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
func hash(into hasher: inout Hasher)
```

## See Also

### Comparing heart rate zone alerts

var hashValue: Int

The hashed value of the heart rate zone alert.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two heart rate zone alerts aren’t equal.

static func == (HeartRateZoneAlert, HeartRateZoneAlert) -> Bool

Returns a Boolean value that indicates whether two heart rate zone alerts are equal.

