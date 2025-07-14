

- WorkoutKit
- WorkoutAlertMetric
-  hashValue 

Instance Property

# hashValue

The hashed value of the workout metric.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
var hashValue: Int { get }
```

## See Also

### Comparing metrics

static func == (WorkoutAlertMetric, WorkoutAlertMetric) -> Bool

Returns a Boolean value that indicates whether two workout metrics are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workout metrics aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of the workout metric by feeding them into the given hash function.

