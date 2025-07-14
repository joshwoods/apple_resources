

- WorkoutKit
- WorkoutAlert
-  power(zone:) 

Type Method

# power(zone:)

Creates a new alert for the specified power zone.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func power(zone: Int) -> Self
```

Available when `Self` is `PowerZoneAlert`.

## Parameters 

`zone`  

The target heart rate zone.

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

struct PowerZoneAlert

An alert for a power zone.

