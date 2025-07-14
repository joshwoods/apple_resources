

- Network Extension
-  NEFilterReport 

Class

# NEFilterReport

The report of the data provider’s action on a flow.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEFilterReport
```

## Overview

The system issues a report by calling your control provider’s handle(_:) method with a report instance when the data provider issues a verdict whose shouldReport property is set to true.

## Topics

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

var bytesInboundCount: Int

The number of inbound bytes received from the flow.

var bytesOutboundCount: Int

The number of outbound bytes sent on the flow.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Flow handling

class NEFilterFlow

The abstract base class for types that represent flows of network data.

class NEFilterBrowserFlow

A flow of network data, originating from a WebKit-based browser, that the filter examines.

class NEFilterSocketFlow

A flow of network data that the filter examines.

class NEFilterNewFlowVerdict

The result from a filter data provder after the initial examination of a flow.

class NEFilterDataVerdict

The result from a filter data provder for subsequent chunks of data on a flow.

class NEFilterControlVerdict

The result from a filter control provider.

class NEFilterRemediationVerdict

The result from a filter data provider after the user requests remediation for a blocked flow.

class NEFilterVerdict

The abstract base class for filter verdict classes.

