

- HealthKit
- HKElectrocardiogram
-  samplingFrequency 

Instance Property

# samplingFrequency

The frequency at which the Apple Watch sampled the voltage.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
@NSCopying
var samplingFrequency: HKQuantity? { get }
```

## Discussion

The system records the frequency in hertz() units.

## See Also

### Accessing Voltage Measurements

var numberOfVoltageMeasurements: Int

The number of voltage measurements associated with this sample.

class VoltageMeasurement

The voltage for all leads at a single point in time.

enum Lead

The lead used to record a voltage measurement.

