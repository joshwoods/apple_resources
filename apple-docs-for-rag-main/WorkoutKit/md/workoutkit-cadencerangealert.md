

- WorkoutKit
-  CadenceRangeAlert 

Structure

# CadenceRangeAlert

An alert for a range of cadence values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct CadenceRangeAlert
```

## Topics

### Creating new cadence range alerts

static func cadence(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Creates a new cadence alert for the target range.

init(target: ClosedRange&lt;Measurement&lt;UnitFrequency>>)

Creates a cadence alert for a closed range of measurements.

### Accessing the alert data

var metric: WorkoutAlertMetric

The metric for the alert.

var target: ClosedRange&lt;Measurement&lt;UnitFrequency>>

The target range.

var targetQuantityLowerBound: HKQuantity

The target’s lower bound.

var targetQuantityUpperBound: HKQuantity

The target’s upper bound.

### Comparing alerts

var hashValue: Int

The hashed value of the cadence range alert.

func hash(into: inout Hasher)

Hashes the essential components of the cadence range alert by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two cadence range alerts aren’t equal.

static func == (CadenceRangeAlert, CadenceRangeAlert) -> Bool

Returns a Boolean value that indicates whether two cadence range alerts are equal.

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

static func cadence(Double, unit: UnitFrequency) -> Self

Creates an alert for the specified cadence threshold.

struct CadenceThresholdAlert

An alert for a cadence threshold.

