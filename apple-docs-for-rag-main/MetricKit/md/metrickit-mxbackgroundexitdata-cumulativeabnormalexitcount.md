

- MetricKit
- MXBackgroundExitData
-  cumulativeAbnormalExitCount 

Instance Property

# cumulativeAbnormalExitCount

The number of times the app exited abnormally from the background.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var cumulativeAbnormalExitCount: Int { get }
```

## Discussion

The most common causes of an abnormal exit are uncaught Objective-C exceptions, calls to an abort function, and other conditions resulting in an abort signal.

