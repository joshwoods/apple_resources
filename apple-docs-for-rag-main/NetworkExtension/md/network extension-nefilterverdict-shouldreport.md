

- Network Extension
- NEFilterVerdict
-  shouldReport 

Instance Property

# shouldReport

A Boolean value that indicates whether to send a report to the control provider when processing this verdict.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var shouldReport: Bool { get set }
```

## Discussion

If the property is equal to true, the system sends a report to the control provider’s handle(_:) method when processing this verdict in the data provider. This property has no effect if the verdict originates in the control provider.

The data provider doesn’t need to wait for a response from the control provider before continuing to process the flow. Therefore, calling the handle(_:) method is a more efficient way to report a flow to the control provider than returning a needRules() verdict.

This property applies when the action taken on a flow is NEFilterAction.allow, NEFilterAction.drop, NEFilterAction.remediate, or NEFilterAction.filterData (the last of which is only for new flows).

