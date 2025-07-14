

- MetricKit
-  MXAppResponsivenessMetric 

Class

# MXAppResponsivenessMetric

An object representing metrics about the responsiveness of the app to user interaction.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXAppResponsivenessMetric
```

## Topics

### Viewing application unresponsive durations

var histogrammedApplicationHangTime: MXHistogram&lt;UnitDuration>

A histogram of the different durations of time in which the app is too busy to handle user interaction responsively.

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

### Responsiveness metrics

class MXAnimationMetric

An object representing metrics about the responsiveness of animation in the app.

class MXAppLaunchMetric

An object representing metrics about app launch time.

class MXHangDiagnostic

An object representing a diagnostic report for an app that is too busy to handle user input responsively.

