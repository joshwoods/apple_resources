

- MetricKit
-  MXGPUMetric 

Class

# MXGPUMetric

An object representing metrics about the use of the GPU.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXGPUMetric
```

## Topics

### Reading GPU use

var cumulativeGPUTime: Measurement&lt;UnitDuration>

The total amount of GPU time used by the app.

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

class MXLocationActivityMetric

An object representing metrics about the use of location-tracking features of a device.

class MXNetworkTransferMetric

An object representing metrics about network transfers.

class MXCPUExceptionDiagnostic

An object representing a diagnostic report for a fatal or nonfatal CPU exception.

