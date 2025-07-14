

- MetricKit
- MXAppRunTimeMetric
-  cumulativeBackgroundLocationTime 

Instance Property

# cumulativeBackgroundLocationTime

The total time the app is in the background and using location services.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var cumulativeBackgroundLocationTime: Measurement { get }
```

## See Also

### Reading application run time

var cumulativeForegroundTime: Measurement&lt;UnitDuration>

The total time the app is in the foreground.

var cumulativeBackgroundTime: Measurement&lt;UnitDuration>

The total time the app is active in the background.

var cumulativeBackgroundAudioTime: Measurement&lt;UnitDuration>

The total time the app is in the background and playing audio.

