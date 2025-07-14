

- MetricKit
-  MXCrashDiagnostic 

Class

# MXCrashDiagnostic

An object representing a diagnostic report for an app crash.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
class MXCrashDiagnostic
```

## Topics

### Viewing exception details

var exceptionType: NSNumber?

The Mach exception type of the crash.

var exceptionCode: NSNumber?

The encoded processor-specific information for the crash.

var signal: NSNumber?

The signal associated with the crash.

var exceptionReason: MXCrashDiagnosticObjectiveCExceptionReason?

var terminationReason: String?

The reason the app was terminated as a human-readable string.

var virtualMemoryRegionInfo: String?

Information about the region of memory an app accessed incorrectly, resulting in a bad-access crash.

### Viewing the call stack

var callStackTree: MXCallStackTree

The call stack for the crash.

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

### Performance metrics

class MXAppLaunchDiagnostic

A diagnostic subclass that encapsulates app launch diagnostic reports.

class MXAppExitMetric

An object representing metrics about the types of foreground and background app exits.

class MXAppRunTimeMetric

An object representing metrics about the amount of time the app is active.

class MXMemoryMetric

An object representing metrics about the app’s memory use.

