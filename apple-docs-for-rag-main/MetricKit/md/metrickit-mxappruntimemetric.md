

- MetricKit
-  MXAppRunTimeMetric 

Class

# MXAppRunTimeMetric

An object representing metrics about the amount of time the app is active.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXAppRunTimeMetric
```

## Topics

### Reading application run time

var cumulativeForegroundTime: Measurement&lt;UnitDuration>

The total time the app is in the foreground.

var cumulativeBackgroundTime: Measurement&lt;UnitDuration>

The total time the app is active in the background.

var cumulativeBackgroundAudioTime: Measurement&lt;UnitDuration>

The total time the app is in the background and playing audio.

var cumulativeBackgroundLocationTime: Measurement&lt;UnitDuration>

The total time the app is in the background and using location services.

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

class MXMemoryMetric

An object representing metrics about the app’s memory use.

class MXCrashDiagnostic

An object representing a diagnostic report for an app crash.

