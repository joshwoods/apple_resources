

- MetricKit
- MXError
-  MXError.Code 

Enumeration

# MXError.Code

Error codes for error values from app metrics.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Launch errors

case launchTaskDuplicated

A task with the same ID has already been started.

case launchTaskInternalFailure

Internal failures happened inside the framework.

case launchTaskInvalidID

The task ID is a `null` value or exceeds the maximum 128 character length.

case launchTaskMaxCount

Exceeded the maximum number of tasks.

case launchTaskPastDeadline

The start call was made too late.

case launchTaskUnknown

The task hasn’t been started or has already been finished.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

class MXMetric

An abstract data class for a metric.

let MXErrorDomain: String

Error domain for error values from app metrics.

struct MXError

Error domain for error handling of app metrics.

class MXCrashDiagnosticObjectiveCExceptionReason

An object that represents the exception reason for an uncaught ObjC exception.

class MXSignpostRecord

An object representing the record for a signpost interval or event.

