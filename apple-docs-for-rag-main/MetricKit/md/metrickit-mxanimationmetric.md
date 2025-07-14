

- MetricKit
-  MXAnimationMetric 

Class

# MXAnimationMetric

An object representing metrics about the responsiveness of animation in the app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class MXAnimationMetric
```

## Topics

### Reading the ratio of scrolling hitch time

var scrollHitchTimeRatio: Measurement&lt;Unit>

The ratio of the time spent hitching while scrolling.

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

class MXAppLaunchMetric

An object representing metrics about app launch time.

class MXAppResponsivenessMetric

An object representing metrics about the responsiveness of the app to user interaction.

class MXHangDiagnostic

An object representing a diagnostic report for an app that is too busy to handle user input responsively.

