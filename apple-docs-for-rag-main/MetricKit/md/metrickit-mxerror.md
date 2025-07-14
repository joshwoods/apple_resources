

- MetricKit
-  MXError 

Structure

# MXError

Error domain for error handling of app metrics.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
struct MXError
```

## Topics

### Getting the error properties

enum Code

Error codes for error values from app metrics.

let MXErrorDomain: String

Error domain for error values from app metrics.

### Getting the launch error properties

static var launchTaskDuplicated: MXError.Code

A task with the same ID has already been started.

static var launchTaskInternalFailure: MXError.Code

Internal failures happened inside the framework.

static var launchTaskInvalidID: MXError.Code

The task ID is a `null` value or exceeds the maximum 128 character length.

static var launchTaskMaxCount: MXError.Code

Exceeded the maximum number of tasks.

static var launchTaskPastDeadline: MXError.Code

The start call was made too late.

static var launchTaskUnknown: MXError.Code

The task hasn’t been started or has already been finished.

enum Code

Error codes for error values from app metrics.

let MXErrorDomain: String

Error domain for error values from app metrics.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
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

enum Code

Error codes for error values from app metrics.

let MXErrorDomain: String

Error domain for error values from app metrics.

class MXCrashDiagnosticObjectiveCExceptionReason

An object that represents the exception reason for an uncaught ObjC exception.

class MXSignpostRecord

An object representing the record for a signpost interval or event.

