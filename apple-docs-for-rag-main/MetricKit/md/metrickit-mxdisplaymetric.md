

- MetricKit
-  MXDisplayMetric 

Class

# MXDisplayMetric

An object representing metrics about the power used to display the app on the screen.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXDisplayMetric
```

## Topics

### Reading average active pixel use

var averagePixelLuminance: MXAverage&lt;MXUnitAveragePixelLuminance>?

The average amount of luminosity of the pixels on an OLED display.

class MXUnitAveragePixelLuminance

A unit of measure of pixel luminosity on an OLED display.

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

class MXGPUMetric

An object representing metrics about the use of the GPU.

class MXLocationActivityMetric

An object representing metrics about the use of location-tracking features of a device.

class MXNetworkTransferMetric

An object representing metrics about network transfers.

class MXCPUExceptionDiagnostic

An object representing a diagnostic report for a fatal or nonfatal CPU exception.

