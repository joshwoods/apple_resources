

- XCTest
- XCTApplicationLaunchMetric
-  init(waitUntilResponsive:) 

Initializer

# init(waitUntilResponsive:)

Initializes a metric that records the time for an app to display its first frame to screen and complete all extended launch tasks, or to display its first frame and wait until the app is responsive.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(waitUntilResponsive: Bool)
```

## Parameters 

`waitUntilResponsive`  

A Boolean that enables the metric to track time until the main thread is responsive after displaying the first frame.

If `false`, the metric tracks time until the app has displayed its first frame and completed all extended launch tasks that extendLaunchMeasurement(forTaskID:) starts.

## See Also

### Related Documentation

class MXMetricManager

The shared object that registers you to receive metrics, creates logs for custom metrics, and gives access to past reports.

### Initializers

init()

Initializes a metric that records the time for an app to display its first frame to screen and complete all extended launch tasks.

