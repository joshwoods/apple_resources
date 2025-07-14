

- MetricKit
- MXAppLaunchMetric
-  histogrammedTimeToFirstDraw 

Instance Property

# histogrammedTimeToFirstDraw

A histogram of the different amounts of time taken to launch the app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var histogrammedTimeToFirstDraw: MXHistogram { get }
```

## See Also

### Viewing app launch and resume time

var histogrammedOptimizedTimeToFirstDraw: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time associated with prewarmed app launches.

var histogrammedApplicationResumeTime: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to resume the app from the background.

var histogrammedExtendedLaunch: MXHistogram&lt;UnitDuration>

A histogram of the different amounts of time taken to launch the app, including the extended launch tasks.

