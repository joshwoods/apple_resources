

- MetricKit
-  MXMemoryMetric 

Class

# MXMemoryMetric

An object representing metrics about the app’s memory use.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXMemoryMetric
```

## Topics

### Measuring memory use

var averageSuspendedMemory: MXAverage&lt;UnitInformationStorage>

The average amount of memory in use by the app when it’s suspended.

var peakMemoryUsage: Measurement&lt;UnitInformationStorage>

The largest amount of memory used by the app.

## Relationships

### Inherits From

- MXMetric

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

class MXCrashDiagnostic

An object representing a diagnostic report for an app crash.

