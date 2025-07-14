

- MetricKit
-  MXLocationActivityMetric 

Class

# MXLocationActivityMetric

An object representing metrics about the use of location-tracking features of a device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXLocationActivityMetric
```

## Topics

### Reading location services use

var cumulativeBestAccuracyForNavigationTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location at the best accuracy for navigation.

var cumulativeBestAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location at the best accuracy.

var cumulativeNearestTenMetersAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location to an accuracy of 10 meters.

var cumulativeHundredMetersAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location to an accuracy of 100 meters.

var cumulativeKilometerAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location to an accuracy of 1 kilometer.

var cumulativeThreeKilometersAccuracyTime: Measurement&lt;UnitDuration>

The total time spent tracking the current location to an accuracy of 3 kilometers.

## Relationships

### Inherits From

- MXMetric

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Battery metrics

class MXCellularConditionMetric

An object representing metrics about the condition of the cellular network.

class MXCPUMetric

An object representing metrics about the use of the CPU.

class MXDisplayMetric

An object representing metrics about the power used to display the app on the screen.

class MXGPUMetric

An object representing metrics about the use of the GPU.

class MXNetworkTransferMetric

An object representing metrics about network transfers.

class MXCPUExceptionDiagnostic

An object representing a diagnostic report for a fatal or nonfatal CPU exception.

