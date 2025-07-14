

- MetricKit
-  MXMetric 

Class

# MXMetric

An abstract data class for a metric.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXMetric
```

## Topics

### Generate a report

func jsonRepresentation() -> Data

Returns the contents of the metric in JSON format.

func dictionaryRepresentation() -> [AnyHashable : Any]

Returns the contents of a metric as a Dictionary.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- MXAnimationMetric
- MXAppExitMetric
- MXAppLaunchMetric
- MXAppResponsivenessMetric
- MXAppRunTimeMetric
- MXCPUMetric
- MXCellularConditionMetric
- MXDiskIOMetric
- MXDisplayMetric
- MXGPUMetric
- MXLocationActivityMetric
- MXMemoryMetric
- MXNetworkTransferMetric
- MXSignpostMetric

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

### Data types

class MXCallStackTree

An object representing the call stack for an exception.

class MXMetaData

An object containing system-level information about the device.

class MXAverage

A unit of measure for an average.

class MXHistogram

An object representing a histogram of data values of the same type of unit.

class MXDiagnostic

An abstract data class for a diagnostic.

enum Code

Error codes for error values from app metrics.

let MXErrorDomain: String

Error domain for error values from app metrics.

struct MXError

Error domain for error handling of app metrics.

class MXCrashDiagnosticObjectiveCExceptionReason

An object that represents the exception reason for an uncaught ObjC exception.

class MXSignpostRecord

An object representing the record for a signpost interval or event.

