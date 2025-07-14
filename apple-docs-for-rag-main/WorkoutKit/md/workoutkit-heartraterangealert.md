

- WorkoutKit
-  HeartRateRangeAlert 

Structure

# HeartRateRangeAlert

An alert for a range of heart rates.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct HeartRateRangeAlert
```

## Topics

### Creating new heart rate alerts

static func heartRate(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Returns a new heart rate alert for the target range.

init(target: ClosedRange&lt;Measurement&lt;UnitFrequency>>)

Creates a new heart rate alert for a closed range of measurements.

### Accessing the alert data

var metric: WorkoutAlertMetric

The metric for the alert.

var target: ClosedRange&lt;Measurement&lt;UnitFrequency>>

The target range.

var targetQuantityLowerBound: HKQuantity

The target’s lower bound.

var targetQuantityUpperBound: HKQuantity

The target’s upper bound.

### Comparing heart rate range alerts

var hashValue: Int

The hashed value of the heart rate range alert.

func hash(into: inout Hasher)

Hashes the essential components of the heart rate range alert by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two heart rate range alerts aren’t equal.

static func == (HeartRateRangeAlert, HeartRateRangeAlert) -> Bool

Returns a Boolean value that indicates whether two heart rate range alerts are equal.

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

### Creating heart rate alerts

static func heartRate(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Creates a new heart rate alert for the target range.

static func heartRate(zone: Int) -> Self

Creates a new alert for the specified heart rate zone.

struct HeartRateZoneAlert

An alert for a heart rate zone.

