

- MetricKit
-  MXHangDiagnostic 

Class

# MXHangDiagnostic

An object representing a diagnostic report for an app that is too busy to handle user input responsively.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
class MXHangDiagnostic
```

## Topics

### Reading total app hang time

var hangDuration: Measurement&lt;UnitDuration>

The amount of time the app is busy and unable to respond to user interaction.

### Viewing the call stack

var callStackTree: MXCallStackTree

The call stack for the app hang report.

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

### Responsiveness metrics

class MXAnimationMetric

An object representing metrics about the responsiveness of animation in the app.

class MXAppLaunchMetric

An object representing metrics about app launch time.

class MXAppResponsivenessMetric

An object representing metrics about the responsiveness of the app to user interaction.

