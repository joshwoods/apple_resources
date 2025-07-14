

- WorkoutKit
-  SpeedThresholdAlert 

Structure

# SpeedThresholdAlert

An alert for a speed threshold.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct SpeedThresholdAlert
```

## Topics

### Creating speed threshold alerts

static func speed(Double, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Returns a new speed threshold alert.

init(target: Measurement&lt;UnitSpeed>, metric: WorkoutAlertMetric)

Creates a new speed threshold alert.

### Accessing alert data

var target: Measurement&lt;UnitSpeed>

A speed measurement that represents the target threshold.

var targetQuantity: HKQuantity

A HealthKit quantity that represents the target speed threshold.

var metric: WorkoutAlertMetric

The metric used to measure the speed.

### Comparing alerts

var hashValue: Int

The hashed value of the speed threshold alert.

func hash(into: inout Hasher)

Hashes the essential components of the speed threshold alert by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two speed threshold alerts aren’t equal.

static func == (SpeedThresholdAlert, SpeedThresholdAlert) -> Bool

Returns a Boolean value that indicates whether two speed threshold alerts are equal.

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

### Creating speed alerts

static func speed(ClosedRange&lt;Double>, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Creates a new speed alert for the provided range.

struct SpeedRangeAlert

An alert for a range of speed values.

static func speed(Double, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Creates a new speed threshold alert.

