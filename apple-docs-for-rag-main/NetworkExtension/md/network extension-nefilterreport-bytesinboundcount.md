

- Network Extension
- NEFilterReport
-  bytesInboundCount 

Instance Property

# bytesInboundCount

The number of inbound bytes received from the flow.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var bytesInboundCount: Int { get }
```

## Discussion

This property is only non-zero when the report event is NEFilterReport.Event.flowClosed.

## See Also

### Getting report properties

var flow: NEFilterFlow?

The flow on which the associated action was taken.

var action: NEFilterAction

The action taken on the reported flow.

enum NEFilterAction

The actions a data provider can take on a filter flow.

var event: NEFilterReport.Event

The type of event indicated by this report.

enum Event

A type that represents the kind of event indicated by a report.

var bytesOutboundCount: Int

The number of outbound bytes sent on the flow.

