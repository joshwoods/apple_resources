

- HealthKit
- HKElectrocardiogram
- HKElectrocardiogram.VoltageMeasurement
-  timeSinceSampleStart 

Instance Property

# timeSinceSampleStart

The time of the measurement relative to the sample’s start time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
var timeSinceSampleStart: TimeInterval { get }
```

## See Also

### Accessing Data

func quantity(for: HKElectrocardiogram.Lead) -> HKQuantity?

Returns the voltage for the specified lead.

