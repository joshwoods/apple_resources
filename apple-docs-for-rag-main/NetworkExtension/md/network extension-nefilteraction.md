

- Network Extension
-  NEFilterAction 

Enumeration

# NEFilterAction

The actions a data provider can take on a filter flow.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
enum NEFilterAction
```

## Overview

The control provider receives a filter report when the data provider issues a verdict with the shouldReport property set to true. The report contains an action property set to one of the values listed here.

## Topics

### Enumeration Cases

case invalid

Invalid action used to represent an error.

case allow

Allow the flow.

case drop

Drop the flow.

case remediate

Remediate the flow.

case filterData

Filter data on the flow.

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

var event: NEFilterReport.Event

The type of event indicated by this report.

enum Event

A type that represents the kind of event indicated by a report.

var bytesInboundCount: Int

The number of inbound bytes received from the flow.

var bytesOutboundCount: Int

The number of outbound bytes sent on the flow.

