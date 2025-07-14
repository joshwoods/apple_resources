

- WorkoutKit
-  SpeedRangeAlert 

Structure

# SpeedRangeAlert

An alert for a range of speed values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct SpeedRangeAlert
```

## Topics

### Creating speed range alerts

static func speed(ClosedRange&lt;Double>, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Returns a new speed alert for the provided range of values.

init(target: ClosedRange&lt;Measurement&lt;UnitSpeed>>, metric: WorkoutAlertMetric)

Creates a new speed alert for the provided range of values.

### Accessing alert data

var target: ClosedRange&lt;Measurement&lt;UnitSpeed>>

The target range of speed measurements.

var targetQuantityLowerBound: HKQuantity

The target range’s lower bounds.

var targetQuantityUpperBound: HKQuantity

The target range’s upper bounds.

var metric: WorkoutAlertMetric

The metric used to measure the speed.

### Comparing alerts

var hashValue: Int

The hashed value of the speed range alert.

func hash(into: inout Hasher)

Hashes the essential components of the speed range alert by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two speed range alerts aren’t equal.

static func == (SpeedRangeAlert, SpeedRangeAlert) -> Bool

Returns a Boolean value that indicates whether two speed range alerts are equal.

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

static func speed(Double, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Creates a new speed threshold alert.

struct SpeedThresholdAlert

An alert for a speed threshold.

