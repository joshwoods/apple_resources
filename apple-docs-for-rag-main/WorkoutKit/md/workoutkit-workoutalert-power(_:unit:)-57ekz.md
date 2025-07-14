

- WorkoutKit
- WorkoutAlert
-  power(\_:unit:) 

Type Method

# power(\_:unit:)

Creates a new power alert for the target range.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func power(
    _ range: ClosedRange,
    unit: UnitPower
) -> Self
```

Available when `Self` is `PowerRangeAlert`.

## Parameters 

`range`  

A closed range of power values.

`unit`  

The power units used by the range values.

## See Also

### Creating power alerts

struct PowerRangeAlert

An alert for a range of power values.

static func power(Double, unit: UnitPower) -> Self

Creates an alert for the specified power threshold.

struct PowerThresholdAlert

An alert for a power threshold.

static func power(zone: Int) -> Self

Creates a new alert for the specified power zone.

struct PowerZoneAlert

An alert for a power zone.

