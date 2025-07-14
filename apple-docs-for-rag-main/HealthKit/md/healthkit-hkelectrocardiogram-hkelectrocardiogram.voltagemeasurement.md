

- HealthKit
- HKElectrocardiogram
-  HKElectrocardiogram.VoltageMeasurement 

Class

# HKElectrocardiogram.VoltageMeasurement

The voltage for all leads at a single point in time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class VoltageMeasurement
```

## Topics

### Accessing Data

func quantity(for: HKElectrocardiogram.Lead) -> HKQuantity?

Returns the voltage for the specified lead.

var timeSinceSampleStart: TimeInterval

The time of the measurement relative to the sample’s start time.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Electrocardiograms

class HKElectrocardiogram

A sample for electrocardiogram data.

