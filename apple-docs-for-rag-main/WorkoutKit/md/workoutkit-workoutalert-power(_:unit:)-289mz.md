

- WorkoutKit
- WorkoutAlert
-  power(\_:unit:) 

Type Method

# power(\_:unit:)

Creates an alert for the specified power threshold.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func power(
    _ value: Double,
    unit: UnitPower
) -> Self
```

Available when `Self` is `PowerThresholdAlert`.

## Parameters 

`value`  

The target power threshold for the alert.

`unit`  

The power units used for the threshold.

## See Also

### Creating power alerts

static func power(ClosedRange&lt;Double>, unit: UnitPower) -> Self

Creates a new power alert for the target range.

struct PowerRangeAlert

An alert for a range of power values.

struct PowerThresholdAlert

An alert for a power threshold.

static func power(zone: Int) -> Self

Creates a new alert for the specified power zone.

struct PowerZoneAlert

An alert for a power zone.

