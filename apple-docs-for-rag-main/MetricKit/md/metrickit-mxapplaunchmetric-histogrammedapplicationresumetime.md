

- MetricKit
- MXAppLaunchMetric
-  histogrammedApplicationResumeTime 

Instance Property

# histogrammedApplicationResumeTime

A histogram of the different amounts of time taken to resume the app from the background.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var histogrammedApplicationResumeTime: MXHistogram { get }
```

## See Also

### Viewing app launch and resume time

var histogrammedOptimizedTimeToFirstDraw: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time associated with prewarmed app launches.

var histogrammedTimeToFirstDraw: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to launch the app.

var histogrammedExtendedLaunch: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to launch the app, including the extended launch tasks.

