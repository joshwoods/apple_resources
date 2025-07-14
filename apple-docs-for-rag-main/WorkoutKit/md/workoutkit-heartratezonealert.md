

- WorkoutKit
-  HeartRateZoneAlert 

Structure

# HeartRateZoneAlert

An alert for a heart rate zone.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct HeartRateZoneAlert
```

## Topics

### Creating new heart rate zone alerts

static func heartRate(zone: Int) -> Self

Returns an alert for the specified heart rate zone.

init(zone: Int)

Creates a new alert for the target heart rate zone.

### Accessing the alert data

var metric: WorkoutAlertMetric

The metric for the alert.

var zone: Int

The target heart rate zone.

### Comparing heart rate zone alerts

var hashValue: Int

The hashed value of the heart rate zone alert.

func hash(into: inout Hasher)

Hashes the essential components of the heart rate zone alert by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two heart rate zone alerts aren’t equal.

static func == (HeartRateZoneAlert, HeartRateZoneAlert) -> Bool

Returns a Boolean value that indicates whether two heart rate zone alerts are equal.

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

struct HeartRateRangeAlert

An alert for a range of heart rates.

static func heartRate(zone: Int) -> Self

Creates a new alert for the specified heart rate zone.

