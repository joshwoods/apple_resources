

- MetricKit
-  MXCallStackTree 

Class

# MXCallStackTree

An object representing the call stack for an exception.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
class MXCallStackTree
```

## Topics

### Generating a report

func jsonRepresentation() -> Data

Returns the contents of the stack tree in JSON format.

## Relationships

### Inherits From

- NSObject

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

class MXMetaData

An object containing system-level information about the device.

class MXAverage

A unit of measure for an average.

class MXHistogram

An object representing a histogram of data values of the same type of unit.

class MXDiagnostic

An abstract data class for a diagnostic.

class MXMetric

An abstract data class for a metric.

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

