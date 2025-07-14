

- Network Extension
-  NEFilterDataVerdict 

Class

# NEFilterDataVerdict

The result from a filter data provder for subsequent chunks of data on a flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEFilterDataVerdict
```

## Overview

Return this verdict type from the various methods of NEFilterDataProvider.

## Topics

### Creating data verdicts

class func allow() -> NEFilterDataVerdict

Creates a verdict that tells the system to pass the current chunk of network data and all subsequent data for the current flow to its final destination.

class func drop() -> NEFilterDataVerdict

Creates a verdict that tells the system to drop the current chunk of network data and all subsequent data for the current flow.

class func pause() -> NEFilterDataVerdict

Creates a verdict that tells the system to pause the flow.

class func remediateVerdict(withRemediationURLMapKey: String?, remediationButtonTextMapKey: String?) -> NEFilterDataVerdict

Creates a verdict to drop the current chunk of network data and all subsequent data for the current flow, and provides a remediation URL.

class func needRules() -> NEFilterDataVerdict

Creates a verdict that tells the system that the Filter Control Provider needs to update the rules before making a decision about the flow’s data.

init(passBytes: Int, peekBytes: Int)

Creates a verdict that tells the system to pass a chunk of network data to its final destination, and specifies the next chunk of data to provide.

### Reporting statistics

var statisticsReportFrequency: NEFilterReport.Frequency

The frequencty at which to provide flow statistics to the data provider.

## Relationships

### Inherits From

- NEFilterVerdict

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

class NEFilterControlVerdict

The result from a filter control provider.

class NEFilterRemediationVerdict

The result from a filter data provider after the user requests remediation for a blocked flow.

class NEFilterVerdict

The abstract base class for filter verdict classes.

class NEFilterReport

The report of the data provider’s action on a flow.

