

- MetricKit
-  MXDiagnostic 

Class

# MXDiagnostic

An abstract data class for a diagnostic.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
class MXDiagnostic
```

## Topics

### Reading data About a diagnostic

var applicationVersion: String

The value of the bundle version key, short form, in the app’s property list.

var metaData: MXMetaData

A set of system-level information for the device.

var signpostData: [MXSignpostRecord]?

### Generating a report

func jsonRepresentation() -> Data

Returns the contents of the diagnostic in JSON format.

func dictionaryRepresentation() -> [AnyHashable : Any]

Returns the contents of a diagnostic as a dictionary.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MXAppLaunchDiagnostic
- MXCPUExceptionDiagnostic
- MXCrashDiagnostic
- MXDiskWriteExceptionDiagnostic
- MXHangDiagnostic

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

