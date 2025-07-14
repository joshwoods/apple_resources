

- MetricKit
- MXAppLaunchMetric
-  histogrammedOptimizedTimeToFirstDraw 

Instance Property

# histogrammedOptimizedTimeToFirstDraw

A histogram of the different amounts of time associated with prewarmed app launches.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+visionOS 1.0+

``` source
var histogrammedOptimizedTimeToFirstDraw: MXHistogram { get }
```

## See Also

### Viewing app launch and resume time

var histogrammedTimeToFirstDraw: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to launch the app.

var histogrammedApplicationResumeTime: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to resume the app from the background.

var histogrammedExtendedLaunch: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to launch the app, including the extended launch tasks.

