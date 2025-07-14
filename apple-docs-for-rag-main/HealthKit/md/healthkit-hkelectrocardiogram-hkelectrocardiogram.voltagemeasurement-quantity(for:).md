

- HealthKit
- HKElectrocardiogram
- HKElectrocardiogram.VoltageMeasurement
-  quantity(for:) 

Instance Method

# quantity(for:)

Returns the voltage for the specified lead.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
func quantity(for lead: HKElectrocardiogram.Lead) -> HKQuantity?
```

## Parameters 

`lead`  

The lead whose voltage you want to read.

## Return Value

A quantity object containing a value in volt units. These values are compatible with any units created using voltUnit(with:).

## See Also

### Accessing Data

var timeSinceSampleStart: TimeInterval

The time of the measurement relative to the sample’s start time.

