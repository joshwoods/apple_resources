

- WorkoutKit
-  PowerZoneAlert 

Structure

# PowerZoneAlert

An alert for a power zone.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
struct PowerZoneAlert
```

## Topics

### Creating power zone alerts

static func power(zone: Int) -> Self

Returns a new power zone alert.

init(zone: Int)

Creates a new power zone alert.

### Accessing alert data

var metric: WorkoutAlertMetric

The metric for the alert.

var zone: Int

The target power zone.

### Comparing alerts

var hashValue: Int

The hashed value of the power zone alert.

func hash(into: inout Hasher)

Hashes the essential components of the power zone alert by feeding them into the given hash function.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two power zone alerts aren’t equal.

static func == (PowerZoneAlert, PowerZoneAlert) -> Bool

Returns a Boolean value that indicates whether two power zone alerts are equal.

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

struct PowerThresholdAlert

An alert for a power threshold.

static func power(zone: Int) -> Self

Creates a new alert for the specified power zone.

