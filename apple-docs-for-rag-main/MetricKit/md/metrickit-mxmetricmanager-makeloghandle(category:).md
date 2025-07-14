

- MetricKit
- MXMetricManager
-  makeLogHandle(category:) 

Type Method

# makeLogHandle(category:)

Returns a log handle used for writing custom metric events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
class func makeLogHandle(category: String) -> OSLog
```

## Parameters 

`category`  

A developer-specified string containing the name of the category of custom metrics written to the log.

## Return Value

A customized OSLog object used for writing custom metrics of the same category.

## Discussion

The object returned by this method saves only custom signpost metrics. Other kinds of os_log messages aren’t persisted.

