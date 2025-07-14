

- MetricKit
-  MXCellularConditionMetric 

Class

# MXCellularConditionMetric

An object representing metrics about the condition of the cellular network.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXCellularConditionMetric
```

## Topics

### Viewing cellular connectivity metrics

var histogrammedCellularConditionTime: MXHistogram&lt;MXUnitSignalBars>

An object representing the distribution of the different levels of connectivity to the cellular network.

class MXUnitSignalBars

A unit of measure for the number of bars of cellular network connectivity.

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

class MXCPUMetric

An object representing metrics about the use of the CPU.

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

