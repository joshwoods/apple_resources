

- Network Extension
-  NEFilterNewFlowVerdict 

Class

# NEFilterNewFlowVerdict

The result from a filter data provder after the initial examination of a flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEFilterNewFlowVerdict
```

## Topics

### Creating new flow verdicts

class func allow() -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that the all of the new flow’s data should be allowed to pass to its final destination.

class func drop() -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that all of the new flow’s data should dropped, and the user should not be given the opportunity to request access.

class func pause() -> NEFilterNewFlowVerdict

Creates a verdict that tells the system to pause the flow.

class func filterDataVerdict(withFilterInbound: Bool, peekInboundBytes: Int, filterOutbound: Bool, peekOutboundBytes: Int) -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that the filter needs to make a decision about a new flow after seeing a portion of the flow’s data.

class func remediateVerdict(withRemediationURLMapKey: String, remediationButtonTextMapKey: String) -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that all of the new flow’s data should be dropped, but allow the user to request access by tapping or clicking on a URL.

class func needRules() -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that the Filter Data Provider needs more information before it can make a decision about a new flow.

class func urlAppendStringVerdict(withMapKey: String) -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that all of the new flow’s data should be allowed to pass to its final destination, but a string should first be appended to the new flow’s request URL.

### Inspecting new flow verdict properties

var statisticsReportFrequency: NEFilterReport.Frequency

The frequency at which the data provider receives reports.

enum Frequency

An enumeration that represents the frequency of filter report delivery.

## Relationships

### Inherits From

- NEFilterVerdict

### Inherited By

- NEFilterControlVerdict

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

class NEFilterDataVerdict

The result from a filter data provder for subsequent chunks of data on a flow.

class NEFilterControlVerdict

The result from a filter control provider.

class NEFilterRemediationVerdict

The result from a filter data provider after the user requests remediation for a blocked flow.

class NEFilterVerdict

The abstract base class for filter verdict classes.

class NEFilterReport

The report of the data provider’s action on a flow.

