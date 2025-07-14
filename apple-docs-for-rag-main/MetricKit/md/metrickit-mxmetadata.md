

- MetricKit
-  MXMetaData 

Class

# MXMetaData

An object containing system-level information about the device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
class MXMetaData
```

## Topics

### Reading data about a payload

var applicationBuildVersion: String

The value of the bundle version key in the app’s property list.

var deviceType: String

The hardware identifier for the device.

var isTestFlightApp: Bool

Indicates whether the app is registered with TestFlight.

var lowPowerModeEnabled: Bool

Indicates whether low power mode is enabled on the device.

var osVersion: String

The version of the OS on the device including the type of OS, version number, and build number.

var platformArchitecture: String

The name of the processor architecture for the device.

var regionFormat: String

The short country code for the region format setting of the device.

var pid: pid_t

The process ID (PID) of the process.

### Generating a report

func jsonRepresentation() -> Data

Returns the contents of the metadata in JSON format.

func dictionaryRepresentation() -> [AnyHashable : Any]

Returns the contents of the metadata as a dictionary.

Deprecated

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

