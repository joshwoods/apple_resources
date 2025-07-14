

- Network Extension
- NEFilterProvider
-  handle(\_:) 

Instance Method

# handle(\_:)

Receives a report from the framework.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func handle(_ report: NEFilterReport)
```

## Parameters 

`report`  

The report delivered from the framework.

## Discussion

The framework calls this method when the data provider extension returns a verdict with the shouldReport property set to true. Override this method in a subclass if you want to handle the flow report.

