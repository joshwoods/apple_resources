

- WorkoutKit
- HeartRateZoneAlert
-  heartRate(zone:) 

Type Method

# heartRate(zone:)

Returns an alert for the specified heart rate zone.

iOS 17.0+iPadOS 17.0+watchOS 10.0+

``` source
static func heartRate(zone: Int) -> Self
```

Available when `Self` is `HeartRateZoneAlert`.

## Parameters 

`zone`  

The target heart rate zone.

## See Also

### Creating new heart rate zone alerts

init(zone: Int)

Creates a new alert for the target heart rate zone.

