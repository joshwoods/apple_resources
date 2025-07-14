

- MetricKit
- MXAppRunTimeMetric
-  cumulativeBackgroundTime 

Instance Property

# cumulativeBackgroundTime

The total time the app is active in the background.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var cumulativeBackgroundTime: Measurement { get }
```

## See Also

### Reading application run time

var cumulativeForegroundTime: Measurement&lt;UnitDuration>

The total time the app is in the foreground.

var cumulativeBackgroundAudioTime: Measurement&lt;UnitDuration>

The total time the app is in the background and playing audio.

var cumulativeBackgroundLocationTime: Measurement&lt;UnitDuration>

The total time the app is in the background and using location services.

