

- Network Extension
-  NEFilterFlow 

Class

# NEFilterFlow

The abstract base class for types that represent flows of network data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEFilterFlow
```

## Topics

### Inspecting flow properties

var url: URL?

The flow’s HTTP URL.

var identifier: UUID

The unique identifier of the flow.

var direction: NETrafficDirection

The initial direction of the flow: incoming or outgoing.

enum NETrafficDirection

A type to represent the direction of network traffic.

var NEFilterFlowBytesMax: UInt64

The maximum number of bytes to pass or peek for a flow.

### Source app identification

var sourceAppUniqueIdentifier: Data?

A byte string that uniquely identifies the binary for each build of the app that is the source of the flow.

var sourceAppIdentifier: String?

A string containing the identifier of the source app of the flow.

var sourceAppVersion: String?

The short version string of the app that is the source of the flow.

var sourceAppAuditToken: Data?

The audit token of the source application of the flow.

var sourceProcessAuditToken: Data?

The audit token of the process that created the flow.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NEFilterBrowserFlow
- NEFilterSocketFlow

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

class NEFilterReport

The report of the data provider’s action on a flow.

