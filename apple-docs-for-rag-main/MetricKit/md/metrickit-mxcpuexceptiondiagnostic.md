

- MetricKit
-  MXCPUExceptionDiagnostic 

Class

# MXCPUExceptionDiagnostic

An object representing a diagnostic report for a fatal or nonfatal CPU exception.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
class MXCPUExceptionDiagnostic
```

## Overview

A CPU exception occurs when your app uses an excessive amount of CPU time over a short period.

## Topics

### Viewing the call stack

var callStackTree: MXCallStackTree

The app call stack associated with the CPU exception.

### Viewing app CPU time

var totalCPUTime: Measurement&lt;UnitDuration>

The total CPU time used during the exception.

var totalSampledTime: Measurement&lt;UnitDuration>

The total time the app was sampled during the exception.

## Relationships

### Inherits From

- MXDiagnostic

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

class MXNetworkTransferMetric

An object representing metrics about network transfers.

