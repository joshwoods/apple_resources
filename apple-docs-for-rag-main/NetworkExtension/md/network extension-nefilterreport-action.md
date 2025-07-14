

- Network Extension
- NEFilterReport
-  action 

Instance Property

# action

The action taken on the reported flow.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var action: NEFilterAction { get }
```

## See Also

### Getting report properties

var flow: NEFilterFlow?

The flow on which the associated action was taken.

enum NEFilterAction

The actions a data provider can take on a filter flow.

var event: NEFilterReport.Event

The type of event indicated by this report.

enum Event

A type that represents the kind of event indicated by a report.

var bytesInboundCount: Int

The number of inbound bytes received from the flow.

var bytesOutboundCount: Int

The number of outbound bytes sent on the flow.

