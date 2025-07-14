

- MetricKit
-  MXAppLaunchMetric 

Class

# MXAppLaunchMetric

An object representing metrics about app launch time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MXAppLaunchMetric
```

## Topics

### Viewing app launch and resume time

var histogrammedOptimizedTimeToFirstDraw: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time associated with prewarmed app launches.

var histogrammedTimeToFirstDraw: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to launch the app.

var histogrammedApplicationResumeTime: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to resume the app from the background.

var histogrammedExtendedLaunch: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to launch the app, including the extended launch tasks.

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

class MXAppResponsivenessMetric

An object representing metrics about the responsiveness of the app to user interaction.

class MXHangDiagnostic

An object representing a diagnostic report for an app that is too busy to handle user input responsively.

