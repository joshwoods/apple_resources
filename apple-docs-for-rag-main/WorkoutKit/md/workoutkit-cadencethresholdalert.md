

- WorkoutKit
-  CadenceThresholdAlert 

Structure

# CadenceThresholdAlert

An alert for a cadence threshold.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct CadenceThresholdAlert
```

## Topics

### Creating new cadence threshold alerts

static func cadence(Double, unit: UnitFrequency) -> Self

Returns a new cadence threshold alert for the target value.

init(target: Measurement&lt;UnitFrequency>)

Create a new cadence threshold alert for the target measurement.

### Accessing the alert data

var metric: WorkoutAlertMetric

The metric for the alert.

var target: Measurement&lt;UnitFrequency>

The target threshold.

var targetQuantity: HKQuantity

A HealthKit quantity that represents the target cadence threshold.

### Comparing cadence threshold alerts

var hashValue: Int

The hashed value of the cadence threshold alert.

func hash(into: inout Hasher)

Hashes the essential components of the cadence threshold alert by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two cadence threshold alerts aren’t equal.

static func == (CadenceThresholdAlert, CadenceThresholdAlert) -> Bool

Returns a Boolean value that indicates whether two cadence threshold alerts are equal.

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

### Creating cadence alerts

static func cadence(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Creates a new alert for a range of cadence values.

struct CadenceRangeAlert

An alert for a range of cadence values.

static func cadence(Double, unit: UnitFrequency) -> Self

Creates an alert for the specified cadence threshold.

