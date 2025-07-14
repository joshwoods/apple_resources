

- MetricKit
-  MXAppLaunchDiagnostic 

Class

# MXAppLaunchDiagnostic

A diagnostic subclass that encapsulates app launch diagnostic reports.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class MXAppLaunchDiagnostic
```

## Topics

### Reading app launch metrics

var callStackTree: MXCallStackTree

The call stack tree associated with the app launch.

var launchDuration: Measurement&lt;UnitDuration>

The total app launch duration.

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

class MXAppExitMetric

An object representing metrics about the types of foreground and background app exits.

class MXAppRunTimeMetric

An object representing metrics about the amount of time the app is active.

class MXMemoryMetric

An object representing metrics about the app’s memory use.

class MXCrashDiagnostic

An object representing a diagnostic report for an app crash.

