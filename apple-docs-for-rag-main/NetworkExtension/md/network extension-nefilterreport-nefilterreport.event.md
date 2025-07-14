

- Network Extension
- NEFilterReport
-  NEFilterReport.Event 

Enumeration

# NEFilterReport.Event

A type that represents the kind of event indicated by a report.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
enum Event
```

## Topics

### Event Types

case newFlow

A type of event indicating the report is for a new flow.

case dataDecision

A type of event indicating the report is about a pass/block decision made after analyzing some amount of a flow’s data.

case flowClosed

A type of event indicating the report is for a flow’s closing.

case statistics

A type of event indicating the report is for the latest statistics of the flow.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var bytesInboundCount: Int

The number of inbound bytes received from the flow.

var bytesOutboundCount: Int

The number of outbound bytes sent on the flow.

