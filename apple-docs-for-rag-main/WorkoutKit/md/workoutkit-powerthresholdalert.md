

- WorkoutKit
-  PowerThresholdAlert 

Structure

# PowerThresholdAlert

An alert for a power threshold.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct PowerThresholdAlert
```

## Topics

### Creating power threshold alerts

static func power(Double, unit: UnitPower) -> Self

Returns a new power threshold alert for the target value.

init(target: Measurement&lt;UnitPower>)

Returns a new power threshold alert for the target measurement.

### Accessing alert data

var metric: WorkoutAlertMetric

The metric for the alert.

var target: Measurement&lt;UnitPower>

The target measurement using power units.

var targetQuantity: HKQuantity

A HealthKit quantity that represents the target power threshold.

### Comparing alerts

var hashValue: Int

The hashed value of the power threshold alert.

func hash(into: inout Hasher)

Hashes the essential components of the power threshold alert by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two power threshold alerts aren’t equal.

static func == (PowerThresholdAlert, PowerThresholdAlert) -> Bool

Returns a Boolean value that indicates whether two power threshold alerts are equal.

### Initializers

init(target: Measurement&lt;UnitPower>, metric: WorkoutAlertMetric)

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

struct PowerRangeAlert

An alert for a range of power values.

static func power(Double, unit: UnitPower) -> Self

Creates an alert for the specified power threshold.

static func power(zone: Int) -> Self

Creates a new alert for the specified power zone.

struct PowerZoneAlert

An alert for a power zone.

