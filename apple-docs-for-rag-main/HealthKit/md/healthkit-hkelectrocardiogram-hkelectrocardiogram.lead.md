

- HealthKit
- HKElectrocardiogram
-  HKElectrocardiogram.Lead 

Enumeration

# HKElectrocardiogram.Lead

The lead used to record a voltage measurement.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
enum Lead
```

## Topics

### Leads

case appleWatchSimilarToLeadI

Apple Watch Series 4 or later.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Voltage Measurements

var numberOfVoltageMeasurements: Int

The number of voltage measurements associated with this sample.

var samplingFrequency: HKQuantity?

The frequency at which the Apple Watch sampled the voltage.

class VoltageMeasurement

The voltage for all leads at a single point in time.

