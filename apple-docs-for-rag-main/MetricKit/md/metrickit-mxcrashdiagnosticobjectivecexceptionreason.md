

- MetricKit
-  MXCrashDiagnosticObjectiveCExceptionReason 

Class

# MXCrashDiagnosticObjectiveCExceptionReason

An object that represents the exception reason for an uncaught ObjC exception.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class MXCrashDiagnosticObjectiveCExceptionReason
```

## Overview

The crash report for an uncaught Objective-C NSException can contain detailed information about the type, name and description of the exception object. Use the properties and methods on MXCrashDiagnosticObjectiveCExceptionReason to access this information.

## Topics

### Generating a report

func dictionaryRepresentation() -> [AnyHashable : Any]

func jsonRepresentation() -> Data

Returns the contents of the exception reason in JSON format.

### Reading the data

var arguments: [String]

var className: String

var composedMessage: String

var exceptionName: String

var exceptionType: String

var formatString: String

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

struct MXError

Error domain for error handling of app metrics.

class MXSignpostRecord

An object representing the record for a signpost interval or event.

