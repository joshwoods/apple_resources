

- MetricKit
-  MXDiagnosticPayload 

Class

# MXDiagnosticPayload

An object that encapsulates a diagnostic report.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
class MXDiagnosticPayload
```

## Overview

The system delivers a diagnostic report as soon as it’s available.

## Topics

### Reading performance metrics

var crashDiagnostics: [MXCrashDiagnostic]?

The diagnostic reports for app crashes during the reporting period.

var cpuExceptionDiagnostics: [MXCPUExceptionDiagnostic]?

The diagnostic reports for fatal and nonfatal CPU exceptions for the app during the reporting period.

### Reading responsiveness metrics

var appLaunchDiagnostics: [MXAppLaunchDiagnostic]?

The diagnostic reports for the app launch time.

var hangDiagnostics: [MXHangDiagnostic]?

The diagnostic reports for times when the app was too busy to handle input responsively during the reporting period.

### Reading disk access metrics

var diskWriteExceptionDiagnostics: [MXDiskWriteExceptionDiagnostic]?

The diagnostic reports for disk write exceptions for the app during the reporting period.

### Generating a report

func jsonRepresentation() -> Data

Returns the contents of the payload in JSON format.

func dictionaryRepresentation() -> [AnyHashable : Any]

Returns the results of the payload as a dictionary.

### Reading information about the payload

var timeStampBegin: Date

The starting time of the reporting period.

var timeStampEnd: Date

The ending time of the reporting period.

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

### Essentials

class MXMetricManager

The shared object that registers you to receive metrics, creates logs for custom metrics, and gives access to past reports.

class MXMetricPayload

An object that encapsulates a daily metrics report.

protocol MXMetricManagerSubscriber

A protocol defining a method for receiving a daily metrics report.

