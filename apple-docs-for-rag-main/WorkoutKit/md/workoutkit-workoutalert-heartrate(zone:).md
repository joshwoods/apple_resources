

- WorkoutKit
- WorkoutAlert
-  heartRate(zone:) 

Type Method

# heartRate(zone:)

Creates a new alert for the specified heart rate zone.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func heartRate(zone: Int) -> Self
```

Available when `Self` is `HeartRateZoneAlert`.

## Parameters 

`zone`  

The target heart rate zone.

## See Also

### Creating heart rate alerts

static func heartRate(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Creates a new heart rate alert for the target range.

struct HeartRateRangeAlert

An alert for a range of heart rates.

struct HeartRateZoneAlert

An alert for a heart rate zone.

