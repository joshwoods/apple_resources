

- MetricKit
- MXAppLaunchMetric
-  histogrammedExtendedLaunch 

Instance Property

# histogrammedExtendedLaunch

A histogram of the different amounts of time taken to launch the app, including the extended launch tasks.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
var histogrammedExtendedLaunch: MXHistogram { get }
```

## See Also

### Viewing app launch and resume time

var histogrammedOptimizedTimeToFirstDraw: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time associated with prewarmed app launches.

var histogrammedTimeToFirstDraw: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to launch the app.

var histogrammedApplicationResumeTime: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to resume the app from the background.

