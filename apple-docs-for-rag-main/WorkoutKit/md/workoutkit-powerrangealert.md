

- WorkoutKit
-  PowerRangeAlert 

Structure

# PowerRangeAlert

An alert for a range of power values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct PowerRangeAlert
```

## Topics

### Creating new power range alerts

static func power(ClosedRange&lt;Double>, unit: UnitPower) -> Self

Returns a new power alert for the target range.

init(target: ClosedRange&lt;Measurement&lt;UnitPower>>)

Creates a new power alert for the target range.

### Accessing the alert value

var metric: WorkoutAlertMetric

The metric for the alert.

var target: ClosedRange&lt;Measurement&lt;UnitPower>>

The target range.

var targetQuantityLowerBound: HKQuantity

The target’s lower bound.

var targetQuantityUpperBound: HKQuantity

The target’s upper bound.

### Comparing alerts

var hashValue: Int

The hashed value of the power range alert.

func hash(into: inout Hasher)

Hashes the essential components of the power range alert by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two power range alerts aren’t equal.

static func == (PowerRangeAlert, PowerRangeAlert) -> Bool

Returns a Boolean value that indicates whether two power range alerts are equal.

### Initializers

init(target: ClosedRange&lt;Measurement&lt;UnitPower>>, metric: WorkoutAlertMetric)

### Default Implementations

Equatable Implementations

WorkoutAlert Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable
- WorkoutAlert

## See Also

### Creating power alerts

static func power(ClosedRange&lt;Double>, unit: UnitPower) -> Self

Creates a new power alert for the target range.

static func power(Double, unit: UnitPower) -> Self

Creates an alert for the specified power threshold.

struct PowerThresholdAlert

An alert for a power threshold.

static func power(zone: Int) -> Self

Creates a new alert for the specified power zone.

struct PowerZoneAlert

An alert for a power zone.

