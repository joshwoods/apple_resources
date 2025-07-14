

- MetricKit
-  MXCPUMetric 

Class

# MXCPUMetric

An object representing metrics about the use of the CPU.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXCPUMetric
```

## Topics

### Reading CPU use

var cumulativeCPUTime: Measurement&lt;UnitDuration>

The total amount of CPU the app used.

var cumulativeCPUInstructions: Measurement&lt;Unit>

The total number of CPU instructions the app executed during the reporting period.

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

class MXDisplayMetric

An object representing metrics about the power used to display the app on the screen.

class MXGPUMetric

An object representing metrics about the use of the GPU.

class MXLocationActivityMetric

An object representing metrics about the use of location-tracking features of a device.

class MXNetworkTransferMetric

An object representing metrics about network transfers.

class MXCPUExceptionDiagnostic

An object representing a diagnostic report for a fatal or nonfatal CPU exception.

