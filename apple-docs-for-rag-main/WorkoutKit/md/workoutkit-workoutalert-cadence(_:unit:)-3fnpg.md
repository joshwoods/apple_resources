

- WorkoutKit
- WorkoutAlert
-  cadence(\_:unit:) 

Type Method

# cadence(\_:unit:)

Creates an alert for the specified cadence threshold.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func cadence(
    _ value: Double,
    unit: UnitFrequency = WorkoutAlertMetric.countPerMinute
) -> Self
```

Available when `Self` is `CadenceThresholdAlert`.

## Parameters 

`value`  

The target cadence threshold for the alert.

`unit`  

The frequency units used for the threshold.

## See Also

### Creating cadence alerts

static func cadence(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Creates a new alert for a range of cadence values.

struct CadenceRangeAlert

An alert for a range of cadence values.

struct CadenceThresholdAlert

An alert for a cadence threshold.

