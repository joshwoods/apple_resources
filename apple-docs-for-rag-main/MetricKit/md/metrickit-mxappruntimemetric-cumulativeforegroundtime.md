

- MetricKit
- MXAppRunTimeMetric
-  cumulativeForegroundTime 

Instance Property

# cumulativeForegroundTime

The total time the app is in the foreground.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var cumulativeForegroundTime: Measurement { get }
```

## See Also

### Reading application run time

var cumulativeBackgroundTime: Measurement&lt;UnitDuration>

The total time the app is active in the background.

var cumulativeBackgroundAudioTime: Measurement&lt;UnitDuration>

The total time the app is in the background and playing audio.

var cumulativeBackgroundLocationTime: Measurement&lt;UnitDuration>

The total time the app is in the background and using location services.

