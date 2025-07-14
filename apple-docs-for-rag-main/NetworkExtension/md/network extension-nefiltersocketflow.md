

- Network Extension
-  NEFilterSocketFlow 

Class

# NEFilterSocketFlow

A flow of network data that the filter examines.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEFilterSocketFlow
```

## Topics

### Getting socket flow properties

var remoteEndpoint: NWEndpoint?

An object containing details about the socket’s remote endpoint.

Deprecated

var remoteHostname: String?

The flow’s remote hostname, if applicable.

class NEFilterFlow

The abstract base class for types that represent flows of network data.

var localEndpoint: NWEndpoint?

An object containing details about the socket’s local endpoint.

Deprecated

var socketFamily: Int32

The protocol family of the socket.

var socketType: Int32

The type of the socket.

var socketProtocol: Int32

The protocol of the socket.

### Instance Properties

var localFlowEndpoint: NWEndpoint?

var remoteFlowEndpoint: NWEndpoint?

## Relationships

### Inherits From

- NEFilterFlow

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

