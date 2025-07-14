

- MetricKit
-  MXNetworkTransferMetric 

Class

# MXNetworkTransferMetric

An object representing metrics about network transfers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXNetworkTransferMetric
```

## Topics

### Reading wireless data use

var cumulativeCellularDownload: Measurement&lt;UnitInformationStorage>

The total amount of data downloaded over the cellular connection.

var cumulativeCellularUpload: Measurement&lt;UnitInformationStorage>

The total amount of data uploaded over the cellular connection.

var cumulativeWifiDownload: Measurement&lt;UnitInformationStorage>

The total amount of data downloaded over the WiFi connection.

var cumulativeWifiUpload: Measurement&lt;UnitInformationStorage>

The total amount of data uploaded over the WiFi connection.

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

class MXLocationActivityMetric

An object representing metrics about the use of location-tracking features of a device.

class MXCPUExceptionDiagnostic

An object representing a diagnostic report for a fatal or nonfatal CPU exception.

