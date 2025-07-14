

- MetricKit
-  MXAppExitMetric 

Class

# MXAppExitMetric

An object representing metrics about the types of foreground and background app exits.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class MXAppExitMetric
```

## Topics

### Reading the foreground exit data

var foregroundExitData: MXForegroundExitData

The metrics for the foreground app exits.

class MXForegroundExitData

An object representing counts for the different types of foreground app exits.

### Reading the background exit data

var backgroundExitData: MXBackgroundExitData

The metrics for the background app exits.

class MXBackgroundExitData

An object representing counts for the different types of background app exits.

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

class MXAppRunTimeMetric

An object representing metrics about the amount of time the app is active.

class MXMemoryMetric

An object representing metrics about the app’s memory use.

class MXCrashDiagnostic

An object representing a diagnostic report for an app crash.

